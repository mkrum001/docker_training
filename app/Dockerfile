FROM alpine

WORKDIR /usr/nodeapp
COPY ./ ./
RUN apk add --update npm
RUN npm install

CMD ["npm", "start"]