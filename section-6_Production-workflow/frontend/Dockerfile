# builder block
FROM node:8-alpine AS builder

WORKDIR '/app'
COPY package.json .
RUN npm install
COPY . .
RUN npm run build

# run block
FROM nginx

COPY --from=builder /app/build /usr/share/nginx/html