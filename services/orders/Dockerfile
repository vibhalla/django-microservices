FROM python:3.6.4-slim

ENV PYTHONUNBUFFERED 1

RUN mkdir /code

WORKDIR /code

COPY . .

RUN pip install -r requirements.txt
CMD ["python3","manage.py","makemigrations"]
CMD ["python3","manage.py","migrate"]
CMD ["python3","manage.py","runserver"]
