FROM python:3.10-alpine
# MAINTAINER Andrii Nefodov

ENV PYTHONUNBUFFERED 1

COPY ./requirements.txt /requirements.txt

RUN pip install -r /requirements.txt

RUN mkdir /app_ex_1
WORKDIR /app_ex_1
COPY ./app_ex_1 /app_ex_1

RUN adduser -D user

USER user
