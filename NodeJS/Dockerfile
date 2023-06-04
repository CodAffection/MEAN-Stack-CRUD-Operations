# Use an official Node runtime as a parent image
FROM node:14-alpine

# Set the working directory to /app
WORKDIR /app

# Copy the package.json and package-lock.json files to the working directory
COPY /NodeJS/package*.json ./

# Install the project dependencies
RUN npm install

# Copy the remaining application code to the working directory
COPY NodeJS .

# Set the command to run when the container starts
CMD ["node", "index.js"]
