# Use an official Node.js runtime as a parent image
FROM node:14

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install Vue.js project dependencies
RUN npm install

# Build the Vue.js project for production
RUN npm run build

# Expose port 8080
EXPOSE 8080

# Serve the Vue.js application
CMD ["npm", "run", "serve"]
