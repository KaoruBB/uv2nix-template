# Minimal uv2nix Template

A minimal template for Python projects using uv2nix and Nix flakes.

## Features

- Simple Python project structure
- uv2nix integration for dependency management
- Nix flake for reproducible development environments

## Getting Started

### Prerequisites

- [Nix](https://nixos.org/download.html) with flakes enabled
- [direnv](https://direnv.net/) (recommended for automatic environment switching)

### Usage

```
# Clone this repository
git clone https://github.com/KaoruBB/uv2nix-template
cd uv2nix-template

# If using direnv:
# Allow .envrc file
direnv allow

# Alternatively, manually enter the development shell:
nix develop

# Run the example
python main.py
```

### Adding Dependencies

1. Run `uv add <package>` to add a new Python package.
2. Update the flake with `direnv reload`

## Project Structure

- `flake.nix`: Nix flake configuration
- `pyproject.toml`: Python project dependencies
- `main.py`: Example Python script
- `uv.lock`: Lock file for Python dependencies
- `.envrc`: direnv configuration for automatic environment activation

## License

MIT
