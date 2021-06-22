# Nodejs-docker-example

This is a brief example about creating a Docker image of a Node.js project, and running it on a local container.

Local requirements:
- Node.js
- Docker


## 1. Local setup

- Go to the project directory and run the following command to install all the dependencies: `npm install`

- To start the server: `npm run start`


## 2. Docker setup

To build the image:

`docker build . -t node-web-app`

To check the container status:

`docker ps`

To run the image:

`docker run -p 8080:8080 -d node-web-app`

Go to localhost:8080 to find if the app is working correctly. You should find a "Hello World" message.

