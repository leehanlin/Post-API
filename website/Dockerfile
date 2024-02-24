# Use an official Node.js runtime as the base image

FROM node:19.6.0-alpine
# Set the working directory within the container
WORKDIR /my-app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Expose the port that your server listens on
EXPOSE 8080

# Command to run the server
CMD ["node", "index.js"]