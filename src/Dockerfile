FROM node:14.17.5
WORKDIR /usr/share/temperatura
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 8080
CMD ["node", "server.js"]%  
