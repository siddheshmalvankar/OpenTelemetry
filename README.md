# OpenTelemetry
Demo on OpenTelemetry and Jaeger Collector




What ?

**Distributed tracing** is the capability for a tracing solution to track and observe service

requests as they flow through distributed systems by collecting data as the requests go

from one service to another.

**OpenTelemetry** is a collection of tools, APIs, and SDKs. Use it to instrument, generate,

collect, and export telemetry data (metrics, logs, and traces) to help you analyze your

software’s performance and behavior.

OpenTelemetry is **generally available** across [several](https://opentelemetry.io/docs/instrumentation/)[ ](https://opentelemetry.io/docs/instrumentation/)[languages](https://opentelemetry.io/docs/instrumentation/)[ ](https://opentelemetry.io/docs/instrumentation/)and is suitable for

use.

CNCF Project

Problem: With a lack of standardization, the net result is the lack of data portability and

the burden on the user to maintain the instrumentation.

The OpenTelemetry project solves these problems by providing a single, vendor-

agnostic solution. The project has broad industry support and adoption from cloud

providers, vendors and end users.

Classification: Public





Components

• Cross-language specification

Describes the cross-language requirements and expectations for all implementations.

•**API:** Defines data types and operations for generating and correlating tracing, metrics, and logging

data.

•**SDK:** Defines requirements for a language-specific implementation of the API. Configuration, data

processing, and exporting concepts are also defined here.

•**Data:** Defines the OpenTelemetry Protocol (OTLP) and vendor-agnostic semantic conventions that

a telemetry backend can provide support for.

• Collector

The OpenTelemetry Collector is a vendor-agnostic proxy that can receive, process, and

export telemetry data. (ex: OTLP, Jaeger, Prometheus, etc)

• Automatic Instrumentation

OpenTelemetry supports a broad number of components that generate relevant telemetry

data from popular libraries and frameworks for supported languages.

Classification: Public





Why?

Classification: Public





Key Concepts:

• **Trace** - an end-to-end trace of an end-user request inside a distributed application;

this trace might include correlating data from multiple services and multiple

processes.

• **Span** - a single, atomic unit of work that occurs inside an application.

• **SpanContext** - a descriptor that is included inside each span which describes this

span’s relationship to its parent span

Classification: Public





How ?

•**API**: Used to generate telemetry data. Follows Open Telemetry Specification

•**SDK**: Implementation of the API with processing and exporting capabilities.

•**Data**: Defines semantic conventions to provide vendor-agnostic implementations as

well as the OpenTelemetry protocol (OTLP).

•**Exporter**: Exports the telemetry data and send it directly or through the collector to

the telemetry backend.

•**Collector**: The vendor-specific or OTLP exporters are used for data filtering,

aggregation, batching, and communication with various telemetry backends.

Classification: Public





Demo

Jager UI: <http://localhost:16686/search>

Grafana UI : <http://localhost:3000/>

Order Service: [http://localhost:5249](http://localhost:5249/)

Classification: Public

Inventory Service: [https://localhost:7101](https://localhost:7101/)





Next Steps

OpenTelemetry support in the Azure SDK for .NET

**Messaging events**: Explore instrumentations for Event Hubs and Service

Bus message creation and check if its traced and correlated with its sending, receiving,

and processing.

<https://github.com/Azure/azure-functions-durable-extension/issues/1578>

Classification: Public

