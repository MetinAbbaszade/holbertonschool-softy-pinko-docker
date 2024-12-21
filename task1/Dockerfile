FROM ubuntu:latest

RUN apt-get update && apt-get upgrade -y

RUN apt-get install -y python python3-pip

RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

RUN pip install flask

WORKDIR /app

COPY app.py /app/

EXPOSE 5252

CMD ["python3", "app.py"]