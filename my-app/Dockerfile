# base image
FROM node:12.2.0-alpine
WORKDIR /app
COPY package*.json /app/
RUN npm install
COPY ./ /app/
RUN npm run build
FROM nginx:alpine
COPY buil/ /usr/share/nginx/html
