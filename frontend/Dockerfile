FROM node:18.17.1

RUN apt-get update && apt-get install -g @vue/cli

RUN mkdir -p /frontend
WORKDIR /frontend

COPY package*.json ./
RUN yarn install
COPY . .

CMD ["yarn", "run", "serve"]