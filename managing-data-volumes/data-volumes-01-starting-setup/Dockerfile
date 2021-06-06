FROM node:14

ARG DEFAULT_PORT=80

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . /app

ENV PORT $DEFAULT_PORT

EXPOSE $PORT

# VOLUME ["/app/node_modules"]

# CMD ["node", "server.js"]
CMD ["npm", "start"]

# docker build -t feedback-node .
# Optional: docker build -t feedback-node --build-arg DEFAULT_PORT=8000 .

# For volumes
# docker run -p 3000:80 -d --name feedback-app --rm -v feedback:/app/feedback feedback-node

# For Bind Mounts
# docker run -p 3000:80 -d --name feedback-app --rm -v feedback:/app/feedback -v "C:\Users\Dell\Documents\Docker\Docker&Kubernetes\managing-data-volumes\data-volumes-01-starting-setup:/app:ro" -v /app/temp -v /app/node_modules feedback-node:volumes

# dockerignore
# Whenever you do not want to add some folder/file to your COPY instruction to build the image

# Env Var
# You can set the PORT in dockerfile OR run command with --env OR in a .env file (need to add [--env-file ./.env] in run command)
# Handling secured data, the best option is to create the .env file, add it to dockerignore, so when you send the image to someone, they do not have acces to this kind of data