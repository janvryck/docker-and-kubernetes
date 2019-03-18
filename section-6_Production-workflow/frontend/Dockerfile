# builder block
FROM node:8-alpine AS builder

WORKDIR '/app'
COPY package.json .
RUN npm install
COPY . .
RUN npm run build

# run block
FROM nginx
EXPOSE 80

COPY --from=builder /app/build /usr/share/nginx/html