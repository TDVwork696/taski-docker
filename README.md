# Проект «taski-docker»

## О проекте:
Проект taski-docker позволяет пользователям создавать список задач, которые они хотят выполнить в течение какого-то времени. После того как они их выполнят, они могут отметить их как выполненные и тогда задачи будут направлены в списко завершённых дел. На базе данного проекта я освовил основные навыки владение Docker. 

## Использованные технологии:
Язык програмирования - Python 3.9.10
Фреймворк DRF
СУБД - postgresql
Docker

## Инструкция для развёртывания проекта:
cd taski-docker
sudo docker compose -f docker-compose.production.yml up -d
sudo docker compose -f docker-compose.production.yml exec backend python manage.py migrate
sudo docker compose -f docker-compose.production.yml exec backend python manage.py collectstatic
sudo docker compose -f docker-compose.production.yml exec backend cp -r /app/collected_static/. /backend_static/static/

## Об авторах:
https://github.com/TDVwork696
