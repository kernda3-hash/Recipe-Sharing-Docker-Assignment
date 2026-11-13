# Use Node.js 18 Alpine as the base image
FROM node:18-alpine

# Set the working directory
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the remaining application files
COPY . .

# Create directory for SQLite database
RUN mkdir -p /app/data

# Expose backend port
EXPOSE 5000

# Start the backend application
CMD ["npm", "start"]