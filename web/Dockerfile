FROM python:3.8.5

ENV PYTHONUNBUFFERED 1

WORKDIR /app

RUN apt-get update && apt-get install -y \
    gettext \
    vim

EXPOSE 8000

COPY requirements.txt ./
RUN pip install -r requirements.txt

COPY . .
