# base image
FROM node
WORKDIR /app
COPY package*.json /app/
RUN npm install
COPY ./ /app/
RUN npm run build
FROM nginx:1.15
COPY /app/build/ /usr/share/nginx/html