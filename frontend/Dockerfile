# Use the official Node.js v20 image as the base
FROM node:23

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Build the app (if necessary)
RUN npm run build

# Expose port (if your app runs on a specific port)
EXPOSE 3000

# Define the command to run your app
CMD ["npm", "start"]
