FROM python:latest

WORKDIR /app

RUN pip install "fastapi[standard]"
# RUN pip install requests

COPY . .

CMD ["fastapi","dev", "/app/src/app.py", "--host", "0.0.0.0"]
