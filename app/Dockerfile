FROM node:18-alpine

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app

COPY index.js package.json package-lock.json ./

RUN npm install --production --retry=5

EXPOSE 3000

CMD ["npm", "start"]