FROM node

WORKDIR /usr/app

# clone locally the repository https://github.com/docker-hy/frontend-example-docker
# build it with node, copy  
COPY . .

RUN npm install \
 && npm run build \
 && npm install -g serve 

EXPOSE 5000

# CMD npm start
CMD ["serve", "-s", "-l", "5000", "dist"]

