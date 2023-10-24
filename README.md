# Kittygram — социальная сеть для обмена фотографиями любимых питомцев.

## Ссылка на соцсеть Kittygram: https://blwol.sytes.net/

## Стек проекта:

- Python 3.9
- Django
- Gunicorn
- Nginx
- Docker
- Django REST Framework

## Запуск проекта:
- Клонируем репозиторий:
```angular2html
git clone git@github.com:blwolhppt/kittygram_final.git
```
- Запускаем:
```angular2html
sudo docker compose -f docker-compose.production.yml up
```
- Выполняем сбор статики и миграции:
```angular2html
sudo docker compose -f docker-compose.production.yml exec backend python manage.py migrate

sudo docker compose -f docker-compose.production.yml exec backend python manage.py collectstatic

sudo docker compose -f docker-compose.production.yml exec backend cp -r /app/collected_static/. /static/static/
```

## Автор проекта: Белова Ольга
