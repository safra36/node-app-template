FROM node:16

WORKDIR /usr/src/app

RUN npm install typescript -g
RUN npm install nodemon -g

COPY package*.json ./
RUN npm install
COPY . .


RUN npm run build

CMD ["node", "dist/main"]

