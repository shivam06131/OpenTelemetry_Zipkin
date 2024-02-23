# Use the official Node.js 18 Alpine image as the base image
FROM node:18-alpine

# Set the working directory
WORKDIR /opt/app-root/src

# Copy package.json and package-lock.json
COPY package*.json ./

# Install app dependencies
RUN npm ci

# Copy the application code into the container
COPY . .

# Expose the port that the app will run on
EXPOSE 6000

# Define the command to run your application
CMD ["npm", "start"]
