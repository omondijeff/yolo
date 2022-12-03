#Define the base image for the client
FROM node

#Define client working directory
WORKDIR /client

#copy package.json to the working directory
COPY package*.json .

#install dependencies
RUN npm install

COPY . .

#Expose port 9090
EXPOSE 9090

#client entry point
CMD ["npm","start"]
