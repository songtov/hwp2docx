# hwp2docx

A Python tool for converting HWP (Hancom Word Processor) files to DOCX format, featuring a modern development setup with Poetry for dependency management.

## 🚀 Features

- Convert single HWP files to DOCX
- Batch convert multiple HWP files in a directory
- Progress tracking for batch conversions
- Error handling and reporting
- Modern development tools:
  - Poetry for dependency management
  - Black for code formatting
  - isort for import sorting
  - ruff for linting
  - pytest for testing

## 📋 Prerequisites

- Python 3.12 or higher
- [Poetry](https://python-poetry.org/docs/) 1.8.3 or higher
- [Poe the Poet](https://poethepoet.natn.io/index.html) for task management

## 🛠️ Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd hwp2docx
   ```

2. Install Poetry (if not already installed):
   ```bash
   pipx install poetry
   ```

3. Install Poe the Poet:
   ```bash
   pipx install poethepoet
   ```

4. Install project dependencies:
   ```bash
   poetry install
   ```

## 🚀 Usage

### Convert a Single File

```bash
poetry run python -m app.main input.hwp -o output.docx
```

### Convert Multiple Files

To convert all HWP files in a directory:
```bash
poetry run python -m app.main /path/to/hwp/files -o /path/to/output
```

### Development

Run the application:
```bash
poetry run poe run
```

Run tests:
```bash
poetry run poe test
```

Watch tests:
```bash
poetry run poe watch-test
```

Run linting:
```bash
poetry run poe lint
```

## 🏗️ Project Structure

```
.
├── app/               # Main application code
│   ├── converter.py  # HWP to DOCX conversion logic
│   └── main.py       # Command-line interface
├── tests/            # Test files
├── pyproject.toml    # Poetry configuration
└── poetry.lock       # Locked dependencies
```

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
