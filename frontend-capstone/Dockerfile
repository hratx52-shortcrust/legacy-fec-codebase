FROM node:current-slim

WORKDIR /usr/src/app

COPY package.json .

RUN npm install

RUN npm run build-prod

COPY . ./

EXPOSE 8081

CMD [ "npm", "start" ]