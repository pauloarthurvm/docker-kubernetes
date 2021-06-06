FROM node:14

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . /app

EXPOSE 80

# VOLUME ["/app/node_modules"]

# CMD ["node", "server.js"]
CMD ["npm", "start"]

# docker build -t feedback-node .

# For volumes
# docker run -p 3000:80 -d --name feedback-app --rm -v feedback:/app/feedback feedback-node

# For Bind Mounts
# docker run -p 3000:80 -d --name feedback-app --rm -v feedback:/app/feedback -v "C:\Users\Dell\Documents\Docker\Docker&Kubernetes\managing-data-volumes\data-volumes-01-starting-setup:/app:ro" -v /app/temp -v /app/node_modules feedback-node:volumes

# dockerignore
# Whenever you do not want to add some folder/file to your COPY instruction to build the image
