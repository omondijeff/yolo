# DevOps Moringa School Week 3 Independent Project

Below are the links to the repositories on Dockerhub

- [Backend](https://hub.docker.com/repository/docker/omondijeff/yolo-backend)

- [Client](https://hub.docker.com/repository/docker/omondijeff/yolo-client)

## Image Choice

I used node image(s) because both the backend and client are node projects.

## Dockerfile Directives

### Backend Dockerfile Directives

`FROM node:alpine
WORKDIR /backend
COPY package*.json .
RUN npm install
COPY . .
EXPOSE 3001
CMD ["npm","start"]`
