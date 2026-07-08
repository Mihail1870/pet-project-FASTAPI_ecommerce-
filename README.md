# FastAPI E-Commerce API

## Краткое описание
Это учебный проект (pet-project) асинхронного REST API для интернет-магазина, разработанный с использованием FastAPI, SQLAlchemy и PostgreSQL. Проект демонстрирует работу с CRUD-операциями, базой данных, авторизацией пользователей, управлением товарами и заказами, пагинацией товаров.

## Для чего проект нужен и какую проблему решает
Этот проект предназначен для обучения созданию бэкенд-сервисов. Он помогает понять, как реализовать основные функции интернет-магазина: добавление товаров, оформление заказов, управление пользователями и аутентификацией.

## 📋 Стек технологий
- Backend: Python 3.9+, FastAPI, Uvicorn

- ORM: SQLAlchemy (Async)

- Database: PostgreSQL

- Auth: JWT (JSON Web Tokens)

- Validation: Pydantic

- Docker — для контейнеризации окружения.

## Установка и запуск

### Требования
- Python 3.9+
- PostgreSQL 16

### Шаги
1. Склонируйте репозиторий:
```bash
git clone https://github.com/Mihail1870/pet-project-FASTAPI_ecommerce-.git
```

2. Перейдите в папку проекта:
```bash
cd pet-project-FASTAPI_ecommerce-
```

3. Настройте параметры подключения к базе данных.
Создайте файл .env в корне проекта на основе шаблона:
```
DATABASE_URL=postgresql+asyncpg://user:password@localhost:5432/ecommerce_db

SECRET_KEY=your_super_secret_key_change_in_production

ALGORITHM=HS256

ACCESS_TOKEN_EXPIRE_MINUTES=30
```
4. Запустите проект:
```bash
docker compose up -d --build
```
Приложение будет доступно по адресу: http://127.0.0.1:8000

Документация API доступна автоматически:

Swagger UI: http://127.0.0.1:8000/docs

ReDoc: http://127.0.0.1:8000/redoc

5. Остановить и удалить контейнеры:
```bash
docker compose down
```
Чтобы удалить также тома (данные БД):
```bash
docker compose down -v
```

### Контакты:
ahtichanov@bk.ru



