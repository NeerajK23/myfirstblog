FROM ubuntu:16.04

MAINTAINER Neeraj Kumar "Smartneeraj.j23.com"
EXPOSE 5000
RUN apt-get update -y
RUN apt-get install -y \
    #libffi-dev \
    #libpq-dev  \
    python3 \
    python-pip \
    python3-dev \
     build-essential

COPY . /app
WORKDIR /app

RUN pip install -r requirements.txt
RUN pip install flask-wtf
RUN pip install flask-sqlalchemy
RUN pip install flask-bcrypt
RUN pip install flask-login
RUN pip install Pillow
RUN pip install flask-mail
ENTRYPOINT ["python"]

CMD ["run.py"]
