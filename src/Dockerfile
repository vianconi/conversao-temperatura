FROM node:20.9.0-alpine3.18
WORKDIR /app
COPY . .
RUN npm install
# en vez de ENTRYPOINT tambien se puede usar ENTRYPOINT 
CMD [ "node", "server.js" ]  