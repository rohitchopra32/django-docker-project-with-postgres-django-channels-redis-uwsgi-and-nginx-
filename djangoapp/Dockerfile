FROM python:3.6-stretch

WORKDIR /djangoapp

ADD  . /djangoapp

RUN pip install -r requirements.txt

EXPOSE 8000
CMD ["uwsgi", "runserver.ini"]
