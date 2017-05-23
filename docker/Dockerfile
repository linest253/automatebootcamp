# Version: 0.0.1
FROM node:0.10
MAINTAINER Tim Lines "tim.lines@alaskaair.com"

# See if you can do this w/o looking at Dockerfile.example
# Create a directory at /usr/src/app

# copy (or add) package.json to /usr/src/app

# copy (or add) app.js to /usr/src/app

# Set the container's working directory to /usr/src/app

# run 'npm install' to install the prerequisties for app.sj

# Open port 3000 into the container

# Specify command to run when the container is launched. 
# Use an array of arguments to avoid issues with `/bin/sh -c`
EXPOSE 8085
RUN mkdir -p /usr/src
WORKDIR /usr/src
RUN git clone https://github.com/automation-tools-bootcamp/example-nodejs-app.git
WORKDIR /usr/src/example-nodejs-app
RUN npm install
CMD [ "npm", "start" ]

# If that worked, try rebuilding in different ways....
