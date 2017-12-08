FROM yarnpkg/node-yarn

COPY ChatVNLaw/ src/app

WORKDIR src/app

RUN yarn install -g

EXPOSE 3000

CMD [ "yarn", "start" ]
