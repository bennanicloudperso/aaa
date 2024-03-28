FROM node:20.12-bookworm-slim

WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
COPY . .

EXPOSE 3000
CMD [ "node", "server.js" ]