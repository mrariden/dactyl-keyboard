FROM python:3.8-slim-buster

RUN apt-get update && \
    apt-get install -y libgl1-mesa-glx gcc bash && \
    rm -rf /var/lib/apt/lists/*

COPY ./requirements.txt .
RUN python -m pip install -r requirements.txt


WORKDIR /app/src
