FROM python:3.11-slim

WORKDIR /app

COPY ./requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY ./app.py .
COPY ./config.py .

CMD ["python", "app.py"]

EXPOSE 5000
