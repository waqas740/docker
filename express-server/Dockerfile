# Create image based off of the official Node 6 image
FROM node:6

# Create a directory where our app will be placed
RUN mkdir -p /app/express

# Change directory so that our commands run inside this new dir
WORKDIR /app/express

# Copy dependency definitions
COPY package.json /app/express/

# Install dependecies
RUN npm install

# Get all the code needed to run the app
#COPY . /app

# Expose the port the app runs in
EXPOSE 3000

# Serve the app
CMD ["npm", "start"]
