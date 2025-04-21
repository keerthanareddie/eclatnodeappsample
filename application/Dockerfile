# Use the lightweight Alpine-based Node.js image
FROM node:16-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to install dependencies first
COPY package.json ./

# Install dependencies
RUN npm install

# Copy the application code into the container
COPY server.js ./

# Expose the port that your app will run on
EXPOSE 3000

# Command to run the app
CMD ["node", "server.js"]
