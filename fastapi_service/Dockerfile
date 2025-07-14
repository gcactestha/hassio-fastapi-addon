FROM python:3.11-alpine

RUN apk add --no-cache mariadb-dev gcc musl-dev     && pip install fastapi uvicorn pymysql

WORKDIR /app
COPY run.py /app/run.py

CMD ["uvicorn", "run:app", "--host", "0.0.0.0", "--port", "8000"]