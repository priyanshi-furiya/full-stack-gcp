# Use official Node.js LTS image
FROM node:18-alpine

# Set working directory inside the container
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install --production

# Copy the rest of your app source code
COPY . .

# Expose the port your app runs on
EXPOSE 3000

# Start the Express app
CMD ["node", "index.js"]
