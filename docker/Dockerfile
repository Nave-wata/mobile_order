FROM python:slim-buster

WORKDIR /usr/src/app

ENV FLASK_APP=app
ENV FLASK_ENV=development

COPY . /usr/src/app/

RUN pip install --upgrade pip
RUN pip install -r requirements.txt