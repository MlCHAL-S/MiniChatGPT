# MiniChatGPT

[![CI/CD](https://github.com/MlCHAL-S/MiniChatGPT/actions/workflows/ci.yml/badge.svg)](https://github.com/MlCHAL-S/MiniChatGPT/actions/workflows/ci.yml)
[![Python Version](https://img.shields.io/badge/python-3.12%2B-blue)](https://www.python.org/)

MiniChatGPT is a simple chatbot application built with Flask and Ollama, designed to simulate a chat interface similar to ChatGPT. The application includes a web interface for user interaction and a backend API to handle chat messages.

---

## Features

- **Chat Interface**: A web-based chat interface built with HTML, CSS, and Bootstrap.
- **API Integration**: Communicates with an API to generate chat responses.
- **Testing**: Comprehensive tests using pytest to ensure the functionality of the chat endpoints.
- **CI/CD Pipeline**: Automated linting, testing, and Docker image building using GitHub Actions.

## Project Structure

- `web/`: Contains the Flask application code.
  - `api.py`: The main API endpoints for the chat application.
  - `templates/`: HTML templates for the web interface.
  - `static/`: Static files like CSS and JavaScript.
- `tests/`: Contains test cases for the application.
  - `test_app.py`: Test cases for the Flask application endpoints.
- `.github/workflows/ci.yml`: GitHub Actions configuration for CI/CD pipeline.
- `requirements.txt`: Python dependencies for the project.
- `README.md`: Project documentation.

## Requirements
- Docker and Docker Compose
- Python venv
- Ubuntu 24.04.1 LTS

## Installation

1. Clone the repository:
```bash
git clone git@github.com:MlCHAL-S/MiniChatGPT.git MiniChatGPT
cd MiniChatGPT
```

2. Create a virtual environment and activate it:
```bash
python -m venv .venv
source .venv/bin/activate
```

3. Install the dependencies:
```bash
pip install -r requirements.txt
```

## Usage
Within the root directory run:
```bash
docker-compose up --build
```
Then visit http://localhost:5000/ in your browser.

## Run tests
```bash
pytest
```