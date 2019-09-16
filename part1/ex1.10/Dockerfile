FROM ubuntu

RUN  apt-get update && apt-get install -y node  

# clone locally the repository https://github.com/docker-hy/frontend-example-docker
COPY config.js package.json package-lock.json README.md src util webpack.config.js .

RUN npm run build && npm install -g serve	

EXPOSE 5000

CMD ["serve", "-s", "-l", "5000", "dist"]

