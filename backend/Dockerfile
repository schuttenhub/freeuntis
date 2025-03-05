FROM node:20-alpine
USER root
RUN apk add --no-cache python3 sqlite py3-pip make g++ \
    && ln -sf python3 /usr/bin/python
RUN mkdir -p /home/node/app/node_modules && chown -R node:node /home/node/app
WORKDIR /home/node/app
USER node
EXPOSE 8000
