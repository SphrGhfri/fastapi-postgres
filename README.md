# SQLAlchemy and FastAPI Template Application

This repository contains a template application using SQLAlchemy and FastAPI, designed for rapid development and deployment. 

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)

## Features

- FastAPI for building web APIs.
- SQLAlchemy for database interactions.
- Docker support for containerized development and deployment.
- Simple and clear project structure.

## Requirements

- Python 3.7+
- Docker (optional, for containerized development)
- Docker Compose (optional, for managing multi-container applications)

## Installation

### Using Docker

1. Clone the repository:
    ```bash
    git clone https://github.com/SphrGhfri/fastapi-postgres.git
    cd fastapi-postgres
    ```

2. Build and run the Docker container:
    ```bash
    docker-compose up --build
    ```

### Manual Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/SphrGhfri/fastapi-postgres.git
    cd fastapi-postgres
    ```

2. Create and activate a virtual environment:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Start the FastAPI application:
    ```bash
    uvicorn main:app --reload
    ```

## Usage

Once the application is running, you can access the FastAPI documentation at `http://localhost:8000/docs` and the OpenAPI schema at `http://localhost:8000/redoc`.

## Project Structure

```plaintext
.
├── .dockerignore
├── .gitignore
├── compose.yaml
├── database.py
├── Dockerfile
├── main.py
├── models.py
├── README.Docker.md
├── README.md
├── requirements.txt
└── schema.py
