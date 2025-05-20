# FastAPI Microservice Template

A modern, production-ready template for building microservices with FastAPI.

## Features

- 🚀 FastAPI framework with modern Python features
- 📝 Pydantic for data validation and settings management
- 🧪 Comprehensive test suite with pytest
- 🔍 Code quality tools (black, isort, mypy, ruff)
- 🔄 Pre-commit hooks for code quality
- 🐳 Docker support
- 🔐 Environment-based configuration
- 📚 API documentation with Swagger UI

## Prerequisites

- Python 3.10+
- Git
- Docker (optional)

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/fastapi-microservice-template.git
   cd fastapi-microservice-template
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up pre-commit hooks:
   ```bash
   pip install pre-commit
   pre-commit install
   ```

5. Run the development server:
   ```bash
   uvicorn main:app --reload
   ```

The API will be available at http://localhost:8000

## API Documentation

- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

## Development

### Running Tests

```bash
pytest
```

### Code Quality

The project uses several tools to maintain code quality:

- **black**: Code formatting
- **isort**: Import sorting
- **mypy**: Static type checking
- **ruff**: Fast Python linter

Run all checks:

```bash
pre-commit run --all-files
```

### Docker Support

Build the Docker image:

```bash
docker build -t fastapi-microservice .
```

Run the container:

```bash
docker run -p 8000:8000 fastapi-microservice
```

## Project Structure

```
fastapi-microservice-template/
├── app/
│   ├── routers/         # API routes
│   │   └── example_router.py
│   ├── services/        # Business logic
│   │   └── example_service.py
│   └── __init__.py
├── tests/
│   ├── routers/         # Route tests
│   │   └── test_example_router.py
│   ├── services/        # Service tests
│   │   └── test_example_service.py
│   └── __init__.py
├── .github/
│   └── workflows/       # GitHub Actions workflows
│       └── ci.yml
├── .pre-commit-config.yaml
├── Dockerfile
├── main.py             # Application entry point
├── pyproject.toml      # Project configuration
└── requirements.txt    # Project dependencies
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details. 