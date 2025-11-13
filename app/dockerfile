FROM node:18-alpine

WORKDIR /app

EXPOSE 3000:3000

COPY package.json ./
COPY yarn.lock ./
COPY ./src ./src
COPY ./spec ./spec

RUN yarn install --production

CMD ["node", "src/index.js"]