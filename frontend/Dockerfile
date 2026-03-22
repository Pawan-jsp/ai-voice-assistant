# Use Node image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy files
COPY frontend/package*.json ./

# Install dependencies
RUN npm install

# Copy all files
COPY frontend/ .

# Build app
RUN npm run build

# Expose port
EXPOSE 3000

# Start app
CMD ["npm", "start"]
