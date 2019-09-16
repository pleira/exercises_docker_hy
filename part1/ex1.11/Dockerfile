FROM node

WORKDIR /usr/app

# clone locally the repository https://github.com/docker-hy/backend-example-docker
COPY . .
RUN npm install

EXPOSE 8000

CMD npm start

