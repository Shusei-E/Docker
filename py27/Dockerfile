# Python 2.7.x

FROM python:2.7.16-buster
USER root

RUN apt-get update
RUN apt-get install -y vim less

RUN pip install --upgrade pip
RUN pip install --upgrade setuptools

# Install packages
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

# $ docker-compose build
# $ docker-compose up
