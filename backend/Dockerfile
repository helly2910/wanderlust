FROM node:21

WORKDIR /app

RUN cd app

COPY package*.json ./
RUN npm i
RUN npm install

COPY . .

COPY .env.sample .env

EXPOSE 5000

ENTRYPOINT ["npm", "start"]
