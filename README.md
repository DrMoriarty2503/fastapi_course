# FastAPI Course

Учебный проект на FastAPI: небольшой REST API для работы с задачами. Репозиторий показывает базовую структуру backend-приложения с роутерами, Pydantic-схемами, SQLAlchemy и асинхронной работой с базой данных.

## Возможности

- Создание задач через API.
- Получение списка задач.
- Валидация входных данных через Pydantic.
- Асинхронная работа с SQLAlchemy.
- Запуск через Uvicorn или Docker.

## Стек

- Python 3.11+
- FastAPI
- SQLAlchemy Async
- Pydantic
- SQLite
- Docker

## Структура проекта

```text
.
├── main.py          # создание FastAPI-приложения
├── router.py        # API-роуты
├── repository.py    # слой работы с данными
├── schemas.py       # Pydantic-схемы
├── database.py      # подключение и модели БД
├── requirements.txt
└── Dockerfile
```

## Быстрый запуск

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
uvicorn main:app --reload
```

Для Windows:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
uvicorn main:app --reload
```

Документация API будет доступна по адресу:

```text
http://127.0.0.1:8000/docs
```

## Docker

```bash
docker build -t fastapi-course .
docker run -p 8000:80 fastapi-course
```

## Статус

Учебный проект для закрепления базовых подходов FastAPI: роутинг, схемы, репозиторий, асинхронная база данных и контейнеризация.
