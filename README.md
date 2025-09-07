# CI/CD Demo

A simple demonstration of Continuous Integration and Continuous Deployment (CI/CD) using GitHub Actions.

## Project Overview

This project contains a basic FastAPI application with unit tests and a GitHub Actions workflow configured to:

1. Run tests automatically on every push or pull request.
2. Ensure code quality and reliability through automated testing.
3. Demonstrate a simple pipeline for CI/CD best practices.

## Features

- FastAPI app with basic functionality.
- Unit tests using `pytest`.
- Automated testing pipeline using GitHub Actions (`.github/workflows/ci.yml`).
- Example of how to set up CI/CD with GitHub.

## Getting Started

### Prerequisites

- Python 3.8+  
- Git  
- (Optional) VS Code or your preferred code editor  

### Running Locally

1. Clone the repository:

```bash
git clone https://github.com/YourUsername/ci-cd-demo.git
cd ci-cd-demo
```
2. Create and activate a virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
3. Install dependencies:
```bash
pip install -r requirements.txt
```
4. Run the FastAPI app:
```bash
uvicorn main:app --reload
```
5. Run tests:
```bash
pytest
```

## CI/CD Pipeline
- The pipeline is defined in .github/workflows/ci.yml.
- On every push or pull request to the main branch, the workflow will:
- Set up Python environment.
- Install dependencies.
- Run unit tests.
- You can see the workflow runs on the Actions tab in your GitHub repository.

## Project Structure
- **main.py** — FastAPI application code.
- **test_main.py** — Unit tests.
- **.github/workflows/ci.yml** — GitHub Actions workflow configuration.
- **requirements.txt** — Python dependencies.
- **README.md** — This documentation.
