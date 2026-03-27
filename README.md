# Blog API (Monolith)

Монолитное приложение на FastAPI с JWT-аутентификацией и PostgreSQL.

## Возможности

- Управление пользователями (регистрация, вход, просмотр/обновление профиля)
- Управление статьями (CRUD)
- Управление комментариями к статьям
- JWT-аутентификация

## Технологический стек

- **Services**: FastAPI, Python 3.11
- **Database**: PostgreSQL 16 
- **ORM**: SQLAlchemy 2.0 (Async)
- **Migrations**: Alembic
- **DevOps**: Docker Compose

## 🚀 Быстрый старт

Для запуска вам понадобятся **Docker** и **Docker Compose**.

1. **Настройка переменных окружения**:
   Создайте файл `.env` на основе примера:
   ```bash
   # Windows
   copy env.example .env
   
   # Linux/Mac
   cp env.example .env
   ```

2. **Запуск приложения**:
   ```bash
   docker-compose up -d
   ```

3. **Миграции применяются автоматически** при старте контейнеров.
   
4. **Остановка**:
   ```bash
   docker-compose down
   ```


- **Полная очистка** (удаление контейнеров и данных баз данных):
  ```bash
  docker-compose down -v
  ```
http://localhost:8000/docs
