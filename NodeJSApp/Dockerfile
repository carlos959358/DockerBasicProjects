# Stage 1: Build
FROM node:24 as build
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
# Add the following line if there's a build step for the app
# RUN npm run build

# Stage 2: Run
FROM node:24-slim
WORKDIR /app
COPY --from=build /app .
EXPOSE 3000
ENV NODE_ENV=production
CMD ["node", "server.js"]
