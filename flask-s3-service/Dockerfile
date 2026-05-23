FROM python:3.11-slim

WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

RUN mkdir -p /tmp && chmod 1777 /tmp

ENV TMPDIR=/tmp

EXPOSE 5001

CMD ["python", "app.py"]