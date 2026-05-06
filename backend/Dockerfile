FROM node:18

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

# injection du secret
ARG API_KEY
ENV API_KEY=$API_KEY

EXPOSE 3001

CMD ["node", "index.js"]