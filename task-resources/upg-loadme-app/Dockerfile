FROM node:14-alpine

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
# both package.json AND package-lock.json are copied

COPY package*.json ./

RUN npm install
# RUN npm ci --only=production

COPY . .

EXPOSE 8081

CMD [ "node", "server.js" ]
