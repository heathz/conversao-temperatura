FROM node
WORKDIR /usr/share/temperatura
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 8080
CMD ["node", "server.js"]%  