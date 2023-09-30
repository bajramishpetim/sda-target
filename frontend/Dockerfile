# Use an official Node.js runtime as a parent image
FROM node:14-alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install app dependencies (including development dependencies)
RUN npm install

# Copy remaining application files to the container
COPY . .

# Expose the port on which the app will run
EXPOSE 3000

# Start the application in development mode using npm run dev
CMD ["npm", "run", "dev"]
