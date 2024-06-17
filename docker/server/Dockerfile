FROM node:18.14-bullseye-slim

ARG GITHUB_NAME
ARG DB_USERNAME
ARG DB_PASSWORD

RUN apt-get update
RUN apt-get install -y git
RUN git clone https://github.com/${GITHUB_NAME}/SocialGameNodeJSServer /usr/games/
WORKDIR /usr/games
RUN npm install
RUN npm install -g forever

