FROM python:3.11-slim

WORKDIR /app

COPY orders/requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY orders/ .

CMD ["python", "app.py"]

EXPOSE 5000
