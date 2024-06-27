# backend/Dockerfile
FROM node:14

WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy the database file
COPY database.db .

# Copy the rest of the application files
COPY . .

EXPOSE 5000
CMD ["node", "server.js"]
