FROM node:10

RUN npm install -g \
  sails

RUN mkdir -p /sails/test-project
WORKDIR /sails
RUN sails new test-project --traditional

WORKDIR /sails/test-project
CMD ["sails", "lift"]


EXPOSE 1337