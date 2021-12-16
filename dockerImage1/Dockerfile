FROM debian
USER root
COPY package.json ./
WORKDIR /
RUN apt-get update
RUN apt-get install -y nodejs
RUN apt-get install -y npm
RUN npm install
COPY . .
ENTRYPOINT node server.js