FROM node:lts-alpine

RUN mkdir /app
WORKDIR /app
COPY package.*json ./

RUN npm install

COPY index.html index.html
COPY public public
COPY src src
COPY vite.config.js vite.config.js

EXPOSE 5173

CMD npm run dev