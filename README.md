# monitoring-stack

[![CI](https://img.shields.io/github/actions/workflow/status/user/monitoring-stack/ci.yml?branch=main)]()
[![Python](https://img.shields.io/badge/python-3.11+-blue.svg)]()
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

> Pre-configured monitoring stack with Prometheus, Grafana, and Alertmanager

A Python project focused on solving real-world engineering problems.

## Features

- **Async Support** — Native asyncio integration with sync fallback
- **Minimal Dependencies** — Only standard library dependencies for core features
- **Comprehensive Logging** — Structured logging with configurable log levels
- **Rich CLI** — Interactive CLI with colored output and progress bars
- **Type Hints** — Full type annotation coverage for IDE support

## Installation

```bash
pip install monitoring-stack
# or
pipx install monitoring-stack
```

## Usage

```python
from monitoring_stack import Client

client = Client(
    timeout=30,
    retries=3,
)

result = client.run()
print(result)
```

## Configuration

Configuration can be provided via environment variables, a config file, or programmatically.

| Variable | Description | Default |
|----------|-------------|--------|
| `MONITORING_STACK_TIMEOUT` | Request timeout in seconds | `30` |
| `MONITORING_STACK_RETRIES` | Number of retry attempts | `3` |
| `MONITORING_STACK_LOG_LEVEL` | Log verbosity (debug, info, warn, error) | `info` |

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
