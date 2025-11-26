# VDE Attendance - Backend

Application FastAPI pour la gestion des présences scolaires.

## Installation

```bash
# Cloner le projet
git clone https://github.com/ALYCIS/vde_attendance.git
cd vde_attendance/backend

#Se placer dans la branche feat/clean-project
git pull origin feat/clean-project
git checkout feat/clean-project

python -m venv venv
venv\Scripts\activate # pour Windows
source venv/bin/activate # Poue mac et linux

pip install uv

uv sync

cp .env.example .env
uv run alembic upgrade head

uv run --active main.py
```

## Docker

```bash
docker-compose up -d
```

## API

- **API** : http://localhost:8000
- **Documentation** : http://localhost:8000/docs
- **PostgreSQL** : localhost:5433
