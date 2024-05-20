# API Final Yatube

API для проекта Yatube, который позволяет взаимодействовать с блогами, комментариями и подписками.

## Установка

### Клонирование репозитория
git clone https://github.com/BrRiff/api_final_yatube.git
cd api_final_yatube

### Создание и активация виртуального окружения
python -m venv venv
source venv/bin/activate  # Для Windows используйте `venv\Scripts\activate`

### Установка зависимостей
pip install -r requirements.txt

### Применение миграций
python manage.py migrate

### Запуск сервера разработки
python manage.py runserver
## Использование

## Примеры API запросов
### Получение списка постов
GET /api/v1/posts/

### Создание нового поста
POST /api/v1/posts/
Content-Type: application/json

{
  "text": "Ваш текст поста",
  "group": 1
}
### Получение списка комментариев к посту
GET /api/v1/posts/{post_id}/comments/

## Тестирование
Для запуска тестов используйте:
pytest

### Стек технологий
Python: 3.9.10
Django: 3.2.16
Django REST Framework: 3.12.4
SQLite (по умолчанию, можно заменить на другую СУБД)

### Спецификация API
После локального запуска проекта спецификацию API можно найти по адресу:
http://localhost:8000/swagger/

### Автор проекта
[BrRiff](https://github.com/BrRiff)
