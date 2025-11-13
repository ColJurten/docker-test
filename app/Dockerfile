FROM node:18-alpine

WORKDIR /app

COPY package.json ./
COPY yarn.lock ./
COPY ./src ./src
COPY ./spec ./spec

RUN yarn install --production

CMD ["node", "src/index.js"]