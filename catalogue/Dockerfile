FROM node:20
# create the /app and set the /app directory
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO_URL="mongodb:/mongodb:27017/catalogue" \
    MONGO="true"
CMD ["node", "server.js;"]