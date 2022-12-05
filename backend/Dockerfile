#Define the base image for the backedn
FROM node:alpine

#Define backend working directory
WORKDIR /backend

#copy package.json to the working directory
COPY package*.json .

#install dependencies
RUN npm install

COPY . .

#Expose port 2020
EXPOSE 3001

#backend entry point
CMD ["npm","start"]
