# base image
FROM node:12.2.0-alpine
WORKDIR /app
COPY . /app
RUN npm install
RUN npm run build
FROM nginx:alpine
COPY build /usr/share/nginx/html
