### YaNews
- Главная страница доступна любому пользователю. На ней отображаются 10 последних новостей и кол-во комментариев к ним.
- Любой пользователь может самостоятельно зарегистрироваться на сайте. Залогиненный (авторизованный) пользователь может оставлять комментарии, редактировать и удалять свои комментарии.
- У каждой новости есть своя страница, с полным текстом новости и комментариями пользователей.
- В коде проекта есть список запрещённых слов, которые нельзя использовать в комментариях.
- Проект на 95% покрыт тестами с помощью библиотеки pytest.

![](https://img.shields.io/badge/Python-3.9-lightblue)
![](https://img.shields.io/badge/Django-3.2-darkgreen)
![](https://img.shields.io/badge/pytest-7.1.3-lightyellow)
![](https://img.shields.io/badge/pytest--django-4.5.2-lightgreen)

<details>
  <summary>Как запустить проект локально</summary>
1. Клонировать репозиторий:

```
git clone git@github.com:ClosedEyeVisuals/ya_news.git
```

2. Cоздать и активировать виртуальное окружение:

```
python -m venv venv
```

```
source venv/Scripts/activate
```

3. Установить зависимости из файла requirements.txt:

```
python -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

4. Выполнить миграции:

```
python manage.py migrate
```

5. Для загрузки заготовленных новостей после применения миграций выполнить команду:
```
python manage.py loaddata news.json
```

6. Запустить проект:

```
python manage.py runserver
```
Проект доступен по адресу https://127.0.0.1:8000.
</details>
