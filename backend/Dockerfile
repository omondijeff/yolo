#Define the base image for the backedn
FROM node:14.18.2-alpine

#Define backend working directory
WORKDIR /backend

#copy package.json to the working directory
COPY package*.json .

#install dependencies
RUN npm install

#Expose port 4040
EXPOSE 2020

#backend entry point
CMD ["npm","start"]
