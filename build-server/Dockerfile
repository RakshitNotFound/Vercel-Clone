FROM ubuntu:focal

RUN apt-get update
RUN apt-get install -y curl
RUN CURL -sl http://deb.nodesource.com/setup_20.x | bash -
RUN apt-get upgrade -y 
RUN apt-get install -y nodejs

RUN apt-get install git -y 

WORKDIR /home/app

COPY main.sh main.sh

ENTRYPOINT [ "/home/app/main.sh" ]
