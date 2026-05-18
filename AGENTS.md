# Agent Guidelines

This file is intended for AI agents assisting with this project.

- The project is an Android/Java gRPC `.proto` generation module based on Gradle.
- The primary source directory for proto definitions is `src/main/proto/`.
- `server.proto` defines the `Ping` service with basic request/response.
- Project uses `com.google.protobuf` and `java` plugins.
- Adhere to **Conventional Commits** for any generated commit messages.
- Always use the `write_file` tool to make changes, never shell commands for file modifications.
- Ensure any new `.proto` files follow proto3 syntax and have appropriate `java_package`, `java_outer_classname`, and `java_multiple_files` options set.
