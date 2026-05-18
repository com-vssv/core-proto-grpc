# Contributing Guidelines

First off, thank you for considering contributing to `core-proto-grpc`! 

## Commit Message Guidelines

This project strictly follows the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) specification. This leads to more readable messages that are easy to follow when looking through the project history, and allows for automated changelog generation and version bumping.

### Structure

Each commit message consists of a **header**, a **body**, and a **footer**. The header has a special format that includes a **type**, a **scope** and a **subject**:

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

### Types

Must be one of the following:

* **feat**: A new feature (e.g. adding a new proto service or message)
* **fix**: A bug fix (e.g. fixing a typo in a field or message name)
* **docs**: Documentation only changes
* **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
* **refactor**: A code change that neither fixes a bug nor adds a feature
* **perf**: A code change that improves performance
* **test**: Adding missing tests or correcting existing tests
* **build**: Changes that affect the build system or external dependencies (example scopes: gradle, maven)
* **ci**: Changes to our CI configuration files and scripts
* **chore**: Other changes that don't modify src or test files
* **revert**: Reverts a previous commit

### Examples

**Adding a new service:**
```
feat(proto): add new order service definitions
```

**Fixing a typo in proto:**
```
fix(server): correct typo in PingResponse message field
```

**Updating build configuration:**
```
build(gradle): bump springGrpcVersion to 1.0.4
```

### Development Workflow

1. Create a branch for your feature or bug fix.
2. Make your changes in the respective `.proto` files.
3. Verify that the project builds successfully by running `./gradlew build`.
4. Commit your changes using Conventional Commits.
5. Push your branch and create a Pull Request.
