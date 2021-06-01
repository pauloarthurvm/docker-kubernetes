FROM node

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . /app

EXPOSE 3000

CMD ["node", "server.js"]

# Build image with name: docker build -t node-task .

# Create Container: docker run -p 3000:3000 -d --rm --name node node-task