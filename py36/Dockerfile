# Python 3.6.9

FROM python:3.6.9-buster
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
