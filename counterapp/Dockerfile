# Selecting a base image
FROM alpine

# Specifying a working folder for the app in the container
WORKDIR /var/nodeapp

# Copying over the package.json
COPY package.json .

# Installing node and dependencies
RUN apk add --update npm
RUN npm install

# Copying the project file into the working folder
COPY . .

# Specifying the start command for the container
CMD ["npm", "start"]