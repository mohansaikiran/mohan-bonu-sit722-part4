# Your Solution

FROM --platform=linux/amd64 python:3.10-slim

WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY /app .

EXPOSE 8000

ENV DATABASE_URL=postgresql://mohanlib_user:1H48KEFFgw6jUUQysvcaXoVI2d0h2cYY@dpg-crotnv3v2p9s739aefng-a.oregon-postgres.render.com/mohanlib

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000", "--app-dir", "/app"]