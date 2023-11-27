оточення:
    poetry add django pymongo psycopg2 mongoengine

створюємо web проєкт:
    django-admin startproject hw10

запуск сервера:
    cd .\hw10\
    py .\manage.py runserver 
((hw10-local-py3.11) C:\Python\GIT\py_web_HW10\hw10>py .\manage.py runserver)

записываем цитаты в базу:
    py add_quotes_to_mongo.py

коннект до бд монго - створюємо utils.py в quotes


для міграції створюємо quotes\models.py
    py .\manage.py makemigrations
    применяем
    py .\manage.py migrate

hw10/db.sqlite3 - наша бд


створюємо utils\maigration.py

додати дані в вд:
    py -m utils.migration

