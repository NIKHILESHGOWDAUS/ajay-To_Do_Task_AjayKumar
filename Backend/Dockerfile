# Use Node.js LTS image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install --omit=dev

# Copy the rest of the code
COPY . .

# Expose backend port
EXPOSE 3501

# Start the server
CMD ["node", "server.js"]

