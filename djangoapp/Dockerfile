FROM python:3.6-stretch

WORKDIR /djangoapp

ADD  . /djangoapp

RUN pip install -r requirements.txt

EXPOSE 8000

CMD python /djangoapp/djangoproject/manage.py makemigrations && python /djangoapp/djangoproject/manage.py migrate && uwsgi runserver.ini

