# Recipe App API

A robust, production-ready REST API for managing recipes, built with Django and Django REST Framework.

## Features

- **User Authentication:** Secure API with token-based authentication
- **Recipe Management:** Create, read, update, and delete recipes
- **Ingredient Management:** Catalog and organize ingredients
- **Tag Support:** Categorize recipes with custom tags
- **Image Upload:** Attach images to recipes
- **Filtering & Sorting:** Advanced query capabilities
- **Test Driven Development:** Comprehensive test coverage
- **PostgreSQL Database:** Reliable data storage
- **Docker Containerization:** Consistent development and deployment environments

## Tech Stack

- Django 3.2
- Django REST Framework 3.12
- PostgreSQL 13
- Docker & Docker Compose
- Python 3.9

## Getting Started

### Prerequisites

- Docker and Docker Compose installed on your system

### Installation

1. Clone the repository:

   ```
   git clone https://github.com/yourusername/recipe-app-api.git
   cd recipe-app-api
   ```

2. Start the Docker containers:

   ```
   docker-compose up
   ```

3. The API will be available at:
   ```
   http://localhost:8000/api/
   ```

## Project Structure

- `app/` - Django project and application code
- `app/core/` - Base application with shared models and utilities
- `Dockerfile` - Docker container configuration
- `docker-compose.yml` - Multi-container Docker setup
- `requirements.txt` - Python dependencies

## Development

### Running Tests

```
docker-compose run --rm app sh -c "python manage.py test"
```

### Code Linting

```
docker-compose run --rm app sh -c "flake8"
```

## API Documentation

API documentation is available at `/api/docs/` when the server is running.
