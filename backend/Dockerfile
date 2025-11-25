FROM node:latest

WORKDIR /app

COPY package.json /app/

RUN npm install

COPY . /app

EXPOSE 80

# docker run --name node-backend --network multi-network -e MONGODB_USERNAME=[username] -p 80:80 -v /path-to-root-folder/backend:/app  -v logs:/app/logs -v /app/node_modules -d --rm node-backend
ENV MONGODB_USERNAME=root

CMD [ "npm", "start" ]
