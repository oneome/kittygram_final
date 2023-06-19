#  Описание проекта

Проект представляет из себя площадку для обмена информацией о своих любимых питомцах.
Вы можете зайти на сайт, просмотреть фотографии и личные достижения питомцев других пользователей. Можете создать карточку своего питомцы, поделиться в ней информацией, добавить фото.

## Технологии:

Python 3.9  
Django 3.10

## Как развернуть проект:
### Добавьте секрет на GitHub:
DOCKER_USERNAME - имя пользователя на DockerHub  
DOCKER_PASSWORD - пароль на DockerHub  
HOST - api адрес вашего сервера  
SSH_KEY - закрытый SSH ключ для вашего сервера  
SSH_PASSPHRASE - пароль для доступа на сервер  
USER - имя пользователя на сервере    
Для получения сообщения в Telegram о успешном деплое также добавьте
TELEGRAM_TO - ID телеграм-аккаунта получателя сообщения  
TELEGRAM_TOKEN - токен вашего телеграмм-бота

### Далее запуште проект в главную ветку
git add .  
git commit.....  
git push  
При пуше в главную ветку сработает триггер. 
Проект автоматически проверится, соберется в котейнеры,
загрузится в DockerHub, откуда скачается на сервер и запуститься  

### Также создайте в корне и заполните .env:
POSTGRES_USER — имя пользователя,  
POSTGRES_PASSWORD — пароль пользователя,  
POSTGRES_DB — имя базы данных.
### а так же переменные для Django-проекта:
DB_HOST=db  
DB_PORT=5432 

## Автор: Прылипко Егор Сергеевич
