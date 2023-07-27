FROM node:14
WORKDIR /app
COPY package.json package-lock.json ./
RUN npm install -f
COPY . .
CMD ["node", "index.js"]
