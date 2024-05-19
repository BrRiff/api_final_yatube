# API Final Yatube

API для проекта Yatube, который позволяет взаимодействовать с блогами, комментариями и подписками.

## Установка

### Клонирование репозитория

```bash
git clone https://github.com/BrRiff/api_final_yatube.git
cd api_final_yatube
Создание и активация виртуального окружения
bash
Копировать код
python -m venv venv
source venv/bin/activate  # Для Windows используйте `venv\Scripts\activate`
Установка зависимостей
bash
Копировать код
pip install -r requirements.txt
Применение миграций
bash
Копировать код
python manage.py migrate
Запуск сервера разработки
bash
Копировать код
python manage.py runserver
Использование
Примеры API запросов
Получение списка постов
http
Копировать код
GET /api/v1/posts/
Создание нового поста
http
Копировать код
POST /api/v1/posts/
Content-Type: application/json

{
  "text": "Ваш текст поста",
  "group": 1
}
Получение списка комментариев к посту
http
Копировать код
GET /api/v1/posts/{post_id}/comments/
Тестирование
Для запуска тестов используйте:

bash
Копировать код
pytest
Дополнительные настройки
Настройка переменных окружения
Создайте файл .env и добавьте необходимые переменные окружения:

env
Копировать код
DEBUG=True
SECRET_KEY=ваш_секретный_ключ
DATABASE_URL=ваша_база_данных
