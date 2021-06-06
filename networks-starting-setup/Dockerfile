FROM node

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

CMD ["node", "app.js"]

# docker build -t favorites-node .

# Create container using the network
# docker run --name favorites -d --rm -p 3000:3000 --network favorites-net favorites-node:latest

# Create a network to containers communicate
# docker network create favorites-net

# Run the DB container within the network
# docker run -d --name mongodb --network favorites-net mongo