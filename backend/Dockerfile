FROM node:current-alpine3.16
# setup workspace
RUN mkdir -p /home/app
WORKDIR /home/app

# install nestjs
RUN npm i -g @nestjs/cli

# copy dependency files
COPY package*.json /home/app/

# install dependencies
RUN npm ci
