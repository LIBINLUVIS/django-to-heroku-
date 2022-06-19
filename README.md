# django-to-heroku-
hosting an django app to heroku steps


1)Adding Requirement.txt files to the project
2)Adding an Procfile to the Project
3)updating the settings.txt file
  - install django_heroku
  - install gunicorn
  - add Procfile - web: gunicorn test.wsgi
  - add to the req.txt file
  - import django_heroku to the top of settings.py
  - STATIC_ROOT = os.path.join(BASE_DIR, 'static') top the bottom of settings.py
  - django_heroku.settings(locals())  top the bottom of settings.py

4)git init
  git add .
  git commit -m "first commit"

  heroku login
  heroku create app_name
  git push heroku master
  heroku run python manage.py migrate


