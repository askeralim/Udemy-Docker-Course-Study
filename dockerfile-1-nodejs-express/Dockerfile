# this same shows how we can extend/change an existing official image from Docker Hub

FROM node:latest
# highly recommend you always pin versions for anything beyond dev/learn

WORKDIR /usr/src/app
# change working directory to root of nginx webhost
# using WORKDIR is preferred to using 'RUN cd /some/path'
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 3000
CMD [ "npm", "start" ]
