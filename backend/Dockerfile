# Base image
FROM node:16

# Set the working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to install dependencies
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

RUN npm install cors

# Expose port for the backend
EXPOSE 5000

# Command to start the backend
CMD ["npm", "start"]
