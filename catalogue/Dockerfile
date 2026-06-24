FROM node:20
WORKDIR /
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
WORKDIR /
CMD ["node","server.js"]