FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install --production

# Copy source code
COPY . .

# Expose port (matches docker-compose: 3100)
EXPOSE 3100

# Start the server
CMD ["npm", "start"]

