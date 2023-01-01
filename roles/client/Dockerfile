#Define the base image for the client
FROM node

#Define client working directory
WORKDIR /client

#copy package.json to the working directory
COPY package*.json .

#install dependencies
RUN npm install

COPY . .

#Expose port 3090
EXPOSE 3000

#client entry point
CMD ["npm","start"]
