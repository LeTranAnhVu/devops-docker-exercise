FROM ubuntu:16.04

RUN apt-get update && apt-get install -y curl && \
    curl -sL https://deb.nodesource.com/setup_10.x | bash && \
    apt-get install -y nodejs  && \
    apt-get purge -y --auto-remove curl && \
    rm -rf /var/lib/apt/lists/*

WORKDIR /frontend-example-docker

COPY ./frontend-example-docker .

RUN npm install && \
    npm install -g serve

ENV API_URL=http://localhost:8000

RUN npm run build

EXPOSE 5000

CMD serve -s -l 5000 dist