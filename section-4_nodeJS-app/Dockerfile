# Specify base img
FROM node:alpine

# Set working directory
WORKDIR /usr/app

# Copy sources to container
COPY ./ ./

# Install deps
RUN npm install

# Default cmd
CMD ["npm", "start"]