FROM mhart/alpine-node:latest

WORKDIR src/app

RUN mkdir build

COPY ChatVNLaw/build/ ./build
COPY ChatVNLaw/server.js .

RUN yarn add express

EXPOSE 3000

CMD [ "node", "server.js" ]
