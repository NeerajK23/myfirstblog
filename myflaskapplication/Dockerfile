FROM ubuntu:16.04

MAINTAINER Neeraj Kumar "Neeraj.Kumar5@cognizant.com"

EXPOSE 5000

RUN apt-get update -y

 

RUN apt-get install -y \
    #libffi-dev \
    #libpq-dev  \
    python3 \
    python-pip \
    python3-dev \
     build-essential
 
#start for python 3.6

#RUN add-apt-repository ppa:jonathonf/python-3.6

#RUN apt-get update

#RUN apt-get install python3.6

#RUN apt-get update

#RUN apt-get install -y software-properties-common vim

#RUN add-apt-repository ppa:jonathonf/python-3.6

#RUN apt-get update

 

#RUN apt-get install -y build-essential python3.6 python3.6-dev python3-pip python3.6-venv

#RUN apt-get install -y git

#RUN apt-get update

#RUN apt-get install python3.6

 

# update pip

#RUN python3.6 -m pip install pip --upgrade

#RUN python3.6 -m pip install wheel

 

#RUN  apt-get install python3.6

#end

COPY . /app

WORKDIR /app

RUN pip install -r requirements.txt

RUN pip install flask-wtf

RUN pip install flask-sqlalchemy

RUN pip install flask-bcrypt

RUN pip install flask-login

ENTRYPOINT ["python"]

CMD ["run.py"]
