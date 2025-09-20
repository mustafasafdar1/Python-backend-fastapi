# FASTAPI Backend for Social Media Application

This repository contains the backend implementation for a social media application built with [FastAPI](https://fastapi.tiangolo.com/). The project aims to provide a scalable, high-performance, and easy-to-use API for social networking features such as user management, posts, comments, and more.

## Features

- **User Authentication & Authorization**: Secure registration, login, and JWT-based authentication.
- **User Profiles**: Create, update, and fetch user profiles.
- **Posts & Comments**: CRUD operations for posts and comments.
- **Social Features**: Like, follow, and friend management.
- **RESTful API**: Well-structured endpoints following REST conventions.
- **Async Support**: Utilizes FastAPI's async capabilities for improved performance.
- **Database Integration**: Easily connect to popular databases (e.g., PostgreSQL, SQLite).
- **Extensible & Modular**: Clean code structure for easy feature addition.

## Getting Started

### Prerequisites

- Python 3.7+
- [poetry](https://python-poetry.org/) or `pip` for dependency management

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mujtabaalmas/Python-backend-fastapi.git
   cd Python-backend-fastapi
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   Or, if using poetry:
   ```bash
   poetry install
   ```

3. **Set environment variables (if any):**
   Create a `.env` file or set variables as needed for database, secret keys, etc.

4. **Run database migrations (if applicable):**
   ```bash
   # For Alembic or other migration tools
   alembic upgrade head
   ```

5. **Start the FastAPI server:**
   ```bash
   uvicorn main:app --reload
   ```

6. **Access the interactive API docs:**
   - Open [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs) (Swagger UI)
   - Or [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc) (ReDoc)

## Project Structure

```
.
├── app/                  # Main application package
│   ├── api/              # API endpoints (routers)
│   ├── core/             # Core configuration, settings
│   ├── models/           # ORM models
│   ├── schemas/          # Pydantic schemas
│   ├── services/         # Business logic
│   └── main.py           # FastAPI entry point
├── tests/                # Test suite
├── requirements.txt      # Python dependencies
├── alembic/              # Database migrations (if used)
├── .env.example          # Example environment variables
└── README.md             # This file
```

## Contributing

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

## Useful Links

- [FastAPI Documentation](https://fastapi.tiangolo.com/)
- [Uvicorn Documentation](https://www.uvicorn.org/)
- [Pydantic Documentation](https://docs.pydantic.dev/)

---
