FROM node:16

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

# Bundle app source
COPY . .

RUN npm install --force
# If you are building your code for production
# RUN npm ci --only=production

ENV PORT=3000
EXPOSE 3000

CMD [ "node", "server.js" ]

