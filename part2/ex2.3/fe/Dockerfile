FROM ubuntu:16.04

RUN apt-get update && apt-get install -y curl

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash

RUN apt-get install -y nodejs

WORKDIR /myapp

COPY ./frontend-example-docker ./frontend-example-docker

WORKDIR ./frontend-example-docker

RUN npm install

RUN npm install -g serve

ENV API_URL=http://localhost:8000

RUN npm run build

EXPOSE 5000

CMD serve -s -l 5000 dist