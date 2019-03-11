# Specify base img
FROM node:alpine

# Set working directory
WORKDIR /usr/app

# Copy pakcage.json
COPY ./package.json ./
# Install deps
RUN npm install
# Copy sources to container
COPY ./ ./

# Default cmd
CMD ["npm", "start"]