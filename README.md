# core-proto-grpc

This package provides the core gRPC Protocol Buffer definitions for the `com.vssv` platform.

## Overview

This project uses Gradle with the `com.google.protobuf` plugin to generate Java gRPC bindings for the `.proto` files defined in `src/main/proto`.

Current defined services:
- `Ping`: A simple service for health checks and simple communication. Contains `SayPing` and `StreamPing` RPCs.

## Building the Project

To build the project and generate the Java gRPC classes:

```bash
./gradlew build
```

## Publishing

This project is configured to publish using the `maven-publish` plugin.

```bash
./gradlew publish
```

## Requirements

- Java 17
- Gradle
