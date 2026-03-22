FROM node:18-alpine

WORKDIR /app

# Copy only package files first (best practice)
COPY frontend/package.json frontend/package-lock.json* ./

# Install dependencies
RUN npm install --legacy-peer-deps

# Copy remaining code
COPY frontend/ .

# Build
RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]
