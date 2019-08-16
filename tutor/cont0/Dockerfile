from python:3.7-slim-stretch

workdir /app
copy . /app

run pip install -r requirements.txt

expose 80

env NAME Dezzpil

cmd python app.py
