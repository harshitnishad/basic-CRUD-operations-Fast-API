
# 🍵 Tea API - Basic CRUD with FastAPI

This is a simple FastAPI project demonstrating basic CRUD operations on a list of tea items. The API allows users to add, view, update, and delete tea records using HTTP endpoints.

## 🚀 Features

- ✅ View all teas
- ➕ Add a new tea
- ✏️ Update an existing tea
- ❌ Delete a tea by ID
- 🌐 Root welcome message

## 🏗️ Project Structure

```bash
project/
├── main.py       # FastAPI application with CRUD operations
└── README.md     # Project documentation
```

## 📦 Requirements

Install FastAPI and Uvicorn to run this project:

```bash
pip install fastapi uvicorn
```

## ▶️ Running the App

To start the FastAPI server:

```bash
uvicorn main:app --reload
```

Navigate to:

- http://127.0.0.1:8000 – Home
- http://127.0.0.1:8000/docs – Swagger API docs

## 📌 Endpoints

| Method | Endpoint       | Description            |
|--------|----------------|------------------------|
| GET    | `/`            | Welcome message        |
| GET    | `/teas`        | Get list of all teas   |
| POST   | `/teas`        | Add a new tea          |
| PUT    | `/teas/{id}`   | Update tea by ID       |
| DELETE | `/teas/{id}`   | Delete tea by ID       |

## 🛠️ Tech Stack

- **FastAPI** – For building APIs
- **Pydantic** – For data validation

## ✍️ Example JSON for POST/PUT

```json
{
  "id": 1,
  "name": "Darjeeling",
  "origin": "India"
}
```

## 📌 Note

- Data is stored in memory (as a Python list), so it's not persistent between runs.
- Suitable for learning and prototyping FastAPI-based APIs.

## 📄 License

MIT License
