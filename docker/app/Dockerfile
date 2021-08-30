FROM node:16.8.0-alpine3.11

# Add git
RUN apk update && apk add --no-cache git bash \
    && mkdir -p /client

VOLUME /client
WORKDIR /client

EXPOSE 3000 3001
