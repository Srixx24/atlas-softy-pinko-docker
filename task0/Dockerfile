#Creates a layer from the lastest ubuntu
FROM ubuntu:latest

#Update APT using apt-get update
RUN apt-get update

#Upgrade currently installed software
RUN apt-get install -y coreutils

#Echo command
CMD [ "echo", "Hello, World!" ]