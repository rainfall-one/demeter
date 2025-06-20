---
tags: [trait, instrumentation, observability]
---

# Instrumentation Trait

## Overview

The Instrumentation Trait provides a standardized interface for collecting, recording, and exporting metrics related to the work done per request and response in PaperClip. This trait enables the integration of observability tools and supports extensible instrumentation strategies for performance monitoring and analysis.

## Key Responsibilities

- Define hooks or interfaces for capturing metrics at the entry and exit points of request/response cycles.
- Support for custom metrics (e.g., work units, latency, throughput).
- Enable integration with observability backends (e.g., OpenTelemetry, Telegraf, Prometheus).
- Ensure minimal performance overhead and high configurability.

## Example Methods

- `onRequestStart(context)`: Invoked at the start of a request.
- `onRequestEnd(context, result)`: Invoked at the end of a request, with result and metrics.
- `exportMetrics(metrics)`: Export collected metrics to the configured backend.

## Usage

Implement this trait in components that handle requests and responses to ensure consistent instrumentation across the system.
