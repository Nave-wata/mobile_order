FROM python:slim-buster

WORKDIR /usr/src/app

ENV FLASK_APP=app
ENV FLASK_ENV=development
ENV DOCKER_BUILDKIT=1

COPY . /usr/src/app/

RUN pip install --upgrade pip && \
	pip install -r requirements.txt && \
	apt-get update && \
	apt-get install -y git openssh-client