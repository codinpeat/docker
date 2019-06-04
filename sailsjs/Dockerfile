FROM node:10

RUN npm install -g \
  sails \
  nodemon \
  forever

RUN mkdir -p /sails/my-project
WORKDIR /sails
RUN sails new my-project --traditional

WORKDIR /sails/my-project
#CMD ["sails", "lift"]
#CMD ["nodemon", "app.js"]
CMD ["forever", "start", "app.js"]

EXPOSE 1337