# FROM node:20 AS builder
# WORKDIR /opt/server
# COPY package.json .
# COPY *.js .
# RUN npm install


FROM node:20
EXPOSE 8080
ENV DB_HOST="localhost"
RUN mkdir /opt/server 
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install
CMD ["node", "index.js"]
# Before best practices implemented
# FROM node:20
# EXPOSE 8080
# ENV DB_HOST="mysql"
# RUN mkdir /opt/server
# WORKDIR /opt/server
# COPY package.json .
# COPY *.js .
# RUN npm install
# CMD ["node", "index.js"]
