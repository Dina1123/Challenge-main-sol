# Use the official Node.js image
FROM node:18-alpine

# Set working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install Node.js dependencies
RUN npm install


# Copy application code
COPY . .

# Build the Nuxt.js application
RUN npm run build

# Expose port 3000
EXPOSE 3000

# Start the Nuxt.js application
CMD ["npm", "run", "start"]
