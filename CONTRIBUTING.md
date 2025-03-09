# Contributing to PDF Compression System

Thank you for your interest in contributing to the PDF Compression System! This document provides guidelines and instructions for contributing to this project.

## Code of Conduct

By participating in this project, you agree to abide by our Code of Conduct. Please be respectful and considerate of others.

## How to Contribute

### Reporting Bugs

If you find a bug, please create an issue with the following information:

- A clear, descriptive title
- Steps to reproduce the bug
- Expected behavior
- Actual behavior
- Screenshots (if applicable)
- Environment details (OS, Python version, etc.)

### Suggesting Enhancements

If you have an idea for an enhancement, please create an issue with the following information:

- A clear, descriptive title
- A detailed description of the enhancement
- Any relevant examples or mockups
- Why this enhancement would be useful

### Pull Requests

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature-name`)
3. Make your changes
4. Run tests to ensure they pass
5. Commit your changes (`git commit -m 'Add some feature'`)
6. Push to the branch (`git push origin feature/your-feature-name`)
7. Create a new Pull Request

#### Pull Request Guidelines

- Follow the coding style of the project
- Include tests for new features or bug fixes
- Update documentation as needed
- Keep pull requests focused on a single change
- Link to relevant issues

## Development Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/pdf-compression-for-ai.git
   cd pdf-compression-for-ai
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the dependency checker:
   ```bash
   ./check_dependencies.py
   ```

## Testing

Run tests using the provided test runner:

```bash
python run_tests.py
```

Or use the integration test script:

```bash
./run_integration_tests.sh
```

## Code Style

This project follows the PEP 8 style guide. We use the following tools for code quality:

- Black for code formatting
- Flake8 for linting
- MyPy for type checking

Run these tools before submitting a pull request:

```bash
black .
flake8
mypy .
```

## Documentation

Please update documentation as needed when making changes. This includes:

- Code comments
- Docstrings
- README.md
- Other documentation files

## License

By contributing to this project, you agree that your contributions will be licensed under the project's MIT License. 