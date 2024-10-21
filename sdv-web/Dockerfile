FROM node:23-alpine

WORKDIR /usr/src/sdv-web
COPY . .

RUN npm install

EXPOSE 3000

CMD ["npm", "run", "dev"]
