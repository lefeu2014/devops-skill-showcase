FROM node:18

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy rest of the app
COPY . .

# Create uploads folder (for container runtime)
RUN mkdir -p uploads

# Expose port
EXPOSE 5000

# Start the app
CMD ["node", "server.js"]
