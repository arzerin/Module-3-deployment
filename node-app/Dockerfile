# Set the base image
FROM node:18

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy the package.json from the local node-app folder into the container's /usr/src/app
COPY node-app/* /usr/src/app 

# Install npm dependencies
RUN npm install

# Copy the rest of the app's source code into the container
COPY node-app/src ./src

# Expose the port that the app will run on
EXPOSE 5001

# Command to run the app
CMD ["node", "src/server.js"]
