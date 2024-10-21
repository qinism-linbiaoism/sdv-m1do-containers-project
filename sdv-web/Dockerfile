FROM node:23-alpine AS base

WORKDIR /usr/src/sdv-web
COPY . .

FROM base AS dev

RUN npm install
CMD ["npm", "run", "dev"]

FROM base AS prod

RUN npm i next
RUN npm run build
CMD ["npm", "run", "start"]
