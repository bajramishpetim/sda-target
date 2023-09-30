# Use an official Node.js runtime as a parent image
FROM node:14-alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy remaining application files to the container
COPY . .

# Expose the port on which the backend will run
EXPOSE 5000

# Start the backend using ts-node
CMD ["ts-node", "index.ts"]
