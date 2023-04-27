# Specify the base image to use for the Docker container
FROM node:12.2.0-alpine

# Set the working directory for the rest of the Dockerfile
WORKDIR app

# Copy the contents of the current directory to the working directory in the container
COPY . .

# Install Node.js dependencies using npm
RUN npm install

# Run tests for the Node.js project
RUN npm run test

# Expose port 8000 to the outside world
EXPOSE 8000

# Set the command to run when the Docker container starts
CMD ["node","app.js"]
