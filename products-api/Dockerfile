FROM node:20-alpine
ENV NODE_ENV=production
WORKDIR /app

COPY package*.json ./
RUN npm ci --omit=dev

COPY src ./src

EXPOSE 4002
ENV PORT=4002 SERVICE_NAME=products-api USERS_API_URL=http://users-api:4001
CMD ["node", "src/app.js"]