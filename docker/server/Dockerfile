FROM node:18.14

ARG GITHUB_NAME
ARG DB_USERNAME
ARG DB_PASSWORD

RUN apt install git -y
RUN git clone https://github.com/${GITHUB_NAME}/SocialGameNodeJSServer /app/ 
VOLUME /app
WORKDIR /app
RUN npm install
RUN npx tsc
RUN set DB_USER=${DB_USERNAME}
RUN set DB_PWD=${DB_PASSWORD
RUN node js/main.js
