FROM node:14-alpine AS build

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY . .


#================================


#FROM gcr.io/distroless/nodejs:14

#WORKDIR /usr/src/app

#COPY --from=build /usr/src/app .

EXPOSE 3001

CMD ["node","server.js"]
