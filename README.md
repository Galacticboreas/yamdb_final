# Blog-API
### Описание
Благодаря этому проекту можно создавать свои посты и просматиривать записи других пользователей.
### Технологии
Python 3.8
Django 3.1.0
### Запуск проекта в dev-режиме
- запуск контейнеров
docker-compose up -d --build
- миграции приложений
docker-compose exec web python manage.py migrate --noinput
- создание администратора сайта
docker-compose exec web python manage.py createsuperuser
- сбор статических данных
docker-compose exec web python manage.py collectstatic --no-input
- заполнение базы постами пользователей
docker-compose exec web python manage.py loaddata fixtures.json

### Автор


Иванов Борис