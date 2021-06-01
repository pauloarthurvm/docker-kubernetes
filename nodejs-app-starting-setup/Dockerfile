FROM node

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . /app

EXPOSE 80

CMD ["node", "server.js"]

#docker run -p 3000:80 -d --rm IMAGE_ID
# -p selects the local and application ports, -d is for detached and --rm remove the container when exits