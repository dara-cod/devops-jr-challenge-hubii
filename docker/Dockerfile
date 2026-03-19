FROM python:3.11-slim

RUN apt-get update && apt-get upgrade -y && apt-get clean

RUN useradd -m appdara

WORKDIR /app

COPY app/requirements.txt .

RUN pip install --no-cache-dir --upgrade pip setuptools wheel \
    && pip install --no-cache-dir -r requirements.txt

COPY app/ .

USER appdara

EXPOSE 8080

CMD ["python", "-m", "uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8080"]