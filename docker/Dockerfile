FROM python:slim-buster

WORKDIR /usr/src/app

COPY . /usr/src/app/

RUN pip install --upgrade pip && \
	pip install -r requirements.txt && \
	apt-get update && \
	apt-get install -y git openssh-client

RUN adduser dev

ENV HOME /home/dev
ENV FLASK_APP=app
ENV FLASK_ENV=development
ENV DOCKER_BUILDKIT=1

USER dev
