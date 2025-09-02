# Workout API

## Overview
This project is a Workout API built with Python and FastAPI. It provides endpoints to manage workouts, athletes, and related data. It's designed to be simple and maintainable.

## Technologies
- Python 3.13.6
- FastAPI
- SQLAlchemy
- PostgreSQL (via asyncpg)
- Pydantic
- Uvicorn
- FastAPI Pagination

## Project Structure
```
workout_api/
├─ atleta/           
├─ categorias/
├─ centro_treinamento/
├─ configs/          
├─ contrib/          
├─ main.py           
└─ routers.py        
```

## Setup

### 1. Clone the repository
```bash
git clone https://github.com/GuiMarobo/api-workout.git
cd api-workout
```

### 2. Create a virtual environment

#### Using pyenv
```bash
pyenv install 3.13.6
pyenv virtualenv 3.13.6 workoutapi-environment
pyenv activate workoutapi-environment
```

#### Using Python venv
```bash
python3 -m venv workoutapi-env
source workoutapi-env/bin/activate  # Linux/macOS
workoutapi-env\Scripts\activate     # Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Running the API
You can run the API using `make`:
```bash
make run
```
The API will start at [http://127.0.0.1:8004](http://127.0.0.1:8004).

## Usage
- Access endpoints via Swagger UI: [http://127.0.0.1:8004/docs](http://127.0.0.1:8004/docs)  
- Health check: [http://127.0.0.1:8004/health](http://127.0.0.1:8004/health)

## Main Endpoints
- `/atleta` — Manage athletes (GET, POST, PATCH, DELETE)
- `/centro_treinamento` — Manage training centers (GET, POST)
- `/categoria` — Manage categories (GET, POST)

## Notes
- You can change the port in the Makefile if needed.  

