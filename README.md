# api_yamdb
REST API для сервиса YaMDb — базы отзывов о фильмах, книгах и музыке. (Коллективный проект 3 студентов Яндекс.Практикум)


## Описание

API для сервиса YaMDb.

Позволяет работать со следующими сущностями:

- Отзывы 

- Коментарии к отзывам

- Пользователи 

- Категории (типы) произведений

- Категории жанров

- Произведения (на которые пишут отзывы)

Развернув проект у себя, Вы можете ознакомиться с документацией к API по ссылке http://localhost:8000/redoc/

## Развертывание проекта 
1. Склонировать репозиторий

2. Создать виртуальное окружение и активировать его
```
python -m venv venv

source venv/Scripts/activate
```
3. Установить необходимые пакеты
```
pip install -r requirements.txt
```
4. Выполнить миграции: из папки */yatube*, содержащей *файл manage.py*, выполнить команду
```
python manage.py migrate
```
5. Запустить проект
```
python manage.py runserver
```
Готово! 

## Участники 
[Sgonchar89](https://github.com/Sgonchar89) - отзывы (Review) и комментарии (Comments): модели и view, эндпойнты, права доступа для запросов. Рейтинги произведений.

[UlianaVo](https://github.com/UlianaVo) - категории (Categories), жанры (Genres) и произведения (Titles): модели, view и эндпойнты для них.

[LasBazza](https://github.com/LasBazza) - управление пользователями (Auth и Users): система регистрации и аутентификации, права доступа, работа с токеном, система подтверждения e-mail.
