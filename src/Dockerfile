FROM node:17-alpine
WORKDIR /src
COPY package*.json ./
RUN npm install
RUN npm audit fix
COPY . .
EXPOSE 8080
CMD ["node", "server.js"]
