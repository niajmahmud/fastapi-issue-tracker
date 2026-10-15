# FastAPI Issue Tracker API

A REST API for managing issues using FastAPI and JSON file storage.

## Features

- Retrieve all issues
- Create a new issue
- Retrieve an issue by ID
- Update an existing issue
- Delete an issue
- Validate request and response data using Pydantic

## Tech Stack

- Python
- FastAPI
- Pydantic
- Uvicorn
- JSON file storage

## Installation

Clone the repository and enter the project directory.

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd fastapi-issue-tracker
```

Create and activate a virtual environment on Windows:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Run the API

```bash
uvicorn app.main:app --reload
```

## API Documentation

Once the server is running, visit:

http://127.0.0.1:8000/docs

## API Endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/api/v1/issues/` | List issues |
| POST | `/api/v1/issues/` | Create an issue |
| GET | `/api/v1/issues/{issue_id}` | Get an issue |
| PUT | `/api/v1/issues/{issue_id}` | Update an issue |
| DELETE | `/api/v1/issues/{issue_id}` | Delete an issue |
