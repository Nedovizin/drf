# Django REST framework приложение

Создать Django REST framework приложение, с переопределённым пользователем и списком организаций в которых он состоит.

## Две модели
Пользователь:
 - Емайл
 - Пароль
 - Фамилия
 - Имя
 - Телефон
 - Аватар(фотография).
 - Связь на список организаций(может быть больше одной)
 - *Базовые поля, кроме логина, django

Организация:
 - Название
 - Описание

## Функционал:
// все запросы делаются через через 
```curl/postman/вебинтерфейс DRF```
1) Создание нового пользователя(регистрация)
2) Авторизация пользователя по емайлу и паролю
3) Редактирование своего профиля (изменение данных в профиле)
4) Вывод списка всех пользователей
5) Вывод одного пользователя по его ID, со списком связанных с ним организаций
5) Добавление новой организации
6) Вывод списка всех организаций

## Дополнительный функционал, по желанию:
1) Аватар/фотография пользователя, картинка должна при загрузке переименовываться [a-zA-Z0-9]. А так же resize(уменьшить) до размеров не больше 200х200 px.
2) <del>Авторизация пользователя должна происходить через JWT, передача приватных данных(изменения профиля), происходят через этот токен. Можно использовать отдельную библиотеку.</del>
3) <del>Добавить unit-test</del>


## Требования:
1) Python 3.8+
2) Проект должен быть залит на Github/Bitbucket и быть публичным.
3) Проект должен быть в виртуальном окружении venv. Должен присутствовать файл со списком используемых в проекте пакетов и их версий.
4) База данных по умолчанию от django: sqlite3