FROM python:3.11-slim

WORKDIR /app

RUN apt update -y

COPY requirements.txt  .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .


RUN pip install --upgrade pip


EXPOSE 4000

CMD ["python", "run.py"]

