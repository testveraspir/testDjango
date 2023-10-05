Проект на Django
1. Создать виртуальное окружение
`python -m venv djangoTest\venv` (за нас это сделал Pycharm)
2. Активируем виртуальное окружение
`cd djangoTest`
`venv\Scripts\activate`
Будет: (venv) djangoTest
3. Установить Django
`pip isntall django` и 
и Обновить requirements.txt:
`pip freeze > requirements.txt`
4. Создать стартовую структуру Djaingo-проекта
`django-admin startproject config .`
5. Тестируем созданный проект (запуск сервера)
`python manage.py runserver`
6. Создаём наше первое приложение (firstapp)
`python manage.py startapp firstapp`
7. Зарегистрируем приложение firstapp
заходим в config/settings.py и добавляем наше приложение
8. Делаем представление (view)
9. Создаём HTML-шаблон (firstapp/templates/index.html)
10. Создаём маршрут (firstapp/urls.py) и urlpatterns
11. Регистрируем маршрут в главном конфигурационном файле проекта (config/urls.py)
12. Перед созданием администратора нам необходимо активировать БД
`python manage.py migrate`
13. Создаём администратора (createsuperuser)
`python manage.py createsuperuser`
14. Изменяем язык админки (config/settings.py)
и, если необходимо, заголовки в firstapp/admin.py
15. Для регистрации новой модели необходимо её созадть в файле вашеприложение/models
Далее выполнить команду `python manage.py makemigrations вашеприложение`
16. Выполнить миграции: `python manage.py migrate вашеприложение`