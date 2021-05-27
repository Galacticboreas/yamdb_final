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

### Адрес сервера
http://www.galacticborey.ml:81/api/v1/
http://www.galacticborey.ml:81/redoc/
http://www.galacticborey.ml:81/swagger/

### Status badge for a workflow
https://github.com/Galacticboreas/yamdb_final/actions/workflows/yamdb_workflow.yaml/badge.svg
