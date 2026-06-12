FROM python:3.11-slim

# 2. Tworzymy folder wewnątrz kontenera, gdzie będą nasze pliki
WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD ["uvicorn", "bridge:app", "--host", "0.0.0.0", "--port", "8000"]