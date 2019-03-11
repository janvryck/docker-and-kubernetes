# Specify base img
FROM node:alpine

# Copy sources to container
COPY ./ ./

# Install deps
RUN npm install

# Default cmd
CMD ["npm", "start"]