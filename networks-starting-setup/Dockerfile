FROM node

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

CMD ["node", "app.js"]

# docker run --name favorites -d --rm -p 3000:3000 favorites-node:latest