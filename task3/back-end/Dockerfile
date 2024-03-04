#Creates a layer from the lastest ubuntu
FROM ubuntu:latest

#Update APT using apt-get update
RUN apt-get update

#Upgrade currently installed software
RUN apt-get install -y coreutils

#Install python3, python3-pip, flask, and flask-cors
RUN apt-get install -y python3 python3-pip
RUN pip3 install flask
RUN pip3 install flask-cors

#Making working directory
WORKDIR /app

#Copy api to docker image
COPY ./api.py /app/api.py

#Forward port
EXPOSE 5252

#Echo command
CMD [ "echo", "Hello, World!" ]