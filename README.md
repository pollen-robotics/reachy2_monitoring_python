# Reachy2 Monitoring (Python)

This repository provides telemetry and performance tracing utilities for the Reachy 2 robot software stack, based on OpenTelemetry and Pyroscope.

## Overview

It includes reusable tools for profiling and exporting trace data, aimed at helping developers observe, debug, and optimize the behavior of ROS 2-based and gRPC-integrated Reachy systems.

### Features

- **OpenTelemetry-based tracing** for gRPC and custom Python logic
- **Pyroscope integration** for continuous performance profiling
- Context management tools for embedding tracing in existing workflows

### Structure

- **`reachy2_monitoring/tracing_helper.py`**  
  Initializes and manages OpenTelemetry tracing sessions and exporters.
  
- **`otel-python-context_fix.py`**  
  Patch or compatibility script for handling context propagation issues in OpenTelemetry.

- **`requirements.txt` & `pyproject.toml`**  
  List dependencies for Python tracing libraries and exporters.

## Dependencies

Uses the OpenTelemetry SDK with optional backends like Pyroscope and OTLP-compatible platforms.

To install dependencies:

```bash
pip install -r requirements.txt
```

## License

This project is licensed under the **Apache License 2.0** – see the `LICENSE` file for details.
