# DevOps Moringa School Week 3 Independent Project

Below are the links to the repositories on Dockerhub

- [Backend](https://hub.docker.com/repository/docker/omondijeff/yolo-backend)

- [Client](https://hub.docker.com/repository/docker/omondijeff/yolo-client)

## Image Choice

I used node image(s) because both the backend and client are node projects.

## Dockerfile Directives

### Backend Dockerfile Directives

`FROM node:alpine`

`WORKDIR /backend`

`COPY package*.json .`

`RUN npm install`

`COPY . .`

`EXPOSE 3001`

`CMD ["npm","start"]`

### Client Dockerfile Directives

`FROM node:alpine`

`WORKDIR /client`

`COPY package*.json .`

`RUN npm install`

`COPY . .`

`EXPOSE 3001`

`CMD ["npm","start"]`

## Docker Compose Networking

On my docker compose file, I have used the default bridge network created by Docker Compose, then went ahead and allocated the necessary ports.

The Client is allocated `3000` and the Backend is allocated `3001`. The MongoDB Service is allocated port `2018:2018`

## Docker Compose Volume Usage

I created a volume and called it `data`, then used it on the mongo service `data:/data/db`

## Git Workflow

I used the Basic Git Workflow, my commits are self explanatory

## Good practices (Image tag naming)

By Looking at the repos on docker hub, you will notice they have v1 tags and they have been named accordingly .
