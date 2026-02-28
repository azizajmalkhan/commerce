# Use official Node image  with the alphin linu as the base image
FROM node:20-alpine

# Create app directory
WORKDIR /use/src/app

# Copy package files ./ --> destination  
COPY package*.json ./  

# Install dependencies  dev dependencies not install only advatage is its keep mdocker image smaller
#RUN npm ci --only=production
RUN npm install

# Copy all files
COPY . .

# Expose app port
EXPOSE 3002

# Start app
CMD ["node", "server.js"]

