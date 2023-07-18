# Specify the base image
FROM node:latest

# Set the working directory inside the container
WORKDIR /app

# Copy the package.json and package-lock.json files to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the entire application to the working directory
COPY . .

# Expose the port on which the application will run
EXPOSE 5000

# Specify the command to run the application
CMD [ "node", "server.js" ]

