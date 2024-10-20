# My Python Project

This is a basic Python project template using `uv` for dependency management and incorporating typechecking. I use all astral.sh tools, and I don't even have python installed system-wide.

## Setup

1. Install `uv` if you haven't already, preferably through a system package manager:

   - On Windows:
     ```
     scoop install uv
     ```
   - On macOS:
     ```
     brew install uv
     ```

2. Create a virtual environment:

   ```
   uv venv
   ```

3. Activate the virtual environment:
   - On Windows:
     ```
     .\venv\Scripts\activate
     ```
   - On macOS and Linux:
     ```
     source venv/bin/activate
     ```

## Installing Dependencies

- To add runtime dependencies:

  ```
  uv add {package-name}
  ```

- To add development dependencies (like library stubs for typechecking):
  ```
  uv add --dev {package-name}
  ```

## Typechecking

This project uses static type checking. To run the typechecker, use:

```
mypy .
```

## Running the Project

```
uv run src/main.py
```
