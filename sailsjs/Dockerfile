FROM node:10

RUN npm install -g \
  sails

RUN mkdir -p /sails/my-project
WORKDIR /sails
RUN sails new my-project --traditional

WORKDIR /sails/my-project
CMD ["sails", "lift"]


EXPOSE 1337