FROM python:3.7-slim

COPY requirements.txt ./app/

WORKDIR /app

RUN pip3 install -r requirements.txt --no-cache-dir

COPY . .

CMD ["gunicorn", "foodgram.wsgi:application", "--bind", "0:8000" ]
