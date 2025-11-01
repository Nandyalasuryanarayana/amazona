FROM node:16-alpine

WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy all backend code
COPY . .

# Expose port
EXPOSE 5000

# Start server
CMD ["node", "server.js"]
