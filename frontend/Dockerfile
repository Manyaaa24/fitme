# Use Node.js official image
FROM node:20-alpine

# Set working directory inside container
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all frontend files
COPY . .

# Expose Vite default port
EXPOSE 5173

# Start the development server
CMD ["npm", "run", "dev", "--", "--host"]
