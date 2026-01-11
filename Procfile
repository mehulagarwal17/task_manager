release: python manage.py collectstatic --noinput
web: gunicorn taskmanagement.wsgi:application --bind 0.0.0.0:$PORT
