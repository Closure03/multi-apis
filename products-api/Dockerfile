FROM node:20-alpine
ENV NODE_ENV=production
WORKDIR /app

COPY package*.json ./
RUN npm ci --omit=dev

COPY src ./src

EXPOSE 4002
<<<<<<< HEAD
ENV PORT=4002 SERVICE_NAME=products-api USERS_API_URL=http://users-api:4001
=======
ENV PORT=4002 SERVICE_NAME=products-api
>>>>>>> 47cde7ba3a4a6d3c61f313819ed5cc781d60defe
CMD ["node", "src/app.js"]