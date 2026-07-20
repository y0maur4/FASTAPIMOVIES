````markdown id="r9m4fa"
# 🎬 FastAPI Movies

A RESTful API built with **Python** and **FastAPI** for managing a movie catalog. This project demonstrates modern backend development practices, including CRUD operations, request validation, and automatic API documentation.

## 📖 Overview

**FastAPI Movies** is a backend application that allows users to manage a collection of movies through a REST API. It serves as a practical project for learning FastAPI, API development, and backend architecture.

## ✨ Features

- 🎥 Create, read, update, and delete movies (CRUD)
- 🔍 Search movies by title or genre
- ✅ Request validation with Pydantic
- ⚡ High-performance API built with FastAPI
- 📄 Interactive Swagger and ReDoc documentation
- 🗄️ Database-ready architecture
- 🧪 Easy to test and extend

## 🛠️ Technologies

- Python 3.x
- FastAPI
- Uvicorn
- Pydantic
- SQLAlchemy (optional)
- SQLite / PostgreSQL (optional)

## 📂 Project Structure

```
FASTAPIMOVIES/
│
├── app/
│   ├── routers/
│   ├── models/
│   ├── schemas/
│   ├── database.py
│   ├── crud.py
│   └── main.py
│
├── tests/
├── requirements.txt
├── README.md
└── .gitignore
```

## 🚀 Getting Started

### Clone the repository

```bash
git clone https://github.com/yourusername/FASTAPIMOVIES.git
```

### Navigate to the project

```bash
cd FASTAPIMOVIES
```

### Create a virtual environment

```bash
python -m venv venv
```

### Activate the environment

**Windows**

```bash
venv\Scripts\activate
```

**macOS/Linux**

```bash
source venv/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

## ▶️ Run the Application

Start the development server:

```bash
uvicorn app.main:app --reload
```

The API will be available at:

```
http://127.0.0.1:8000
```

## 📚 API Documentation

FastAPI automatically generates interactive documentation.

### Swagger UI

```
http://127.0.0.1:8000/docs
```

### ReDoc

```
http://127.0.0.1:8000/redoc
```

## 🎬 Example Endpoint

```python
from fastapi import FastAPI

app = FastAPI()

movies = [
    {"id": 1, "title": "Inception", "genre": "Sci-Fi"},
    {"id": 2, "title": "The Dark Knight", "genre": "Action"}
]

@app.get("/movies")
def get_movies():
    return movies
```

### Example Response

```json
[
  {
    "id": 1,
    "title": "Inception",
    "genre": "Sci-Fi"
  },
  {
    "id": 2,
    "title": "The Dark Knight",
    "genre": "Action"
  }
]
```

## 📖 Topics Covered

- FastAPI Fundamentals
- REST API Development
- CRUD Operations
- Path & Query Parameters
- Request Body Validation
- Pydantic Models
- API Routing
- Error Handling
- Dependency Injection
- SQLAlchemy Integration
- Database CRUD
- API Documentation
- Testing APIs

## 📦 Requirements

```text
fastapi
uvicorn
pydantic
sqlalchemy
```

Install manually:

```bash
pip install fastapi uvicorn pydantic sqlalchemy
```

## 🎯 Learning Objectives

- Build RESTful APIs using FastAPI.
- Understand API routing and validation.
- Perform CRUD operations efficiently.
- Structure scalable backend applications.
- Integrate APIs with relational databases.

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repository, submit pull requests, or open issues.

## 📄 License

This project is licensed under the MIT License.

## 👨‍💻 Author

Developed as part of a Python Backend and FastAPI learning journey, focusing on API development and software engineering best practices.
````
