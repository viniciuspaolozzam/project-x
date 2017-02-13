FROM node:latest

MAINTAINER Vinicius Paolozza

RUN mkdir /opt/app && \
    apt-get update && \
    apt-get install -y build-essential && \
    apt-get install -y curl && \
    curl -sL https://deb.nodesource.com/setup_5.x | bash - && \
    apt-get install -y nodejs && \
    npm update && \
    npm install gulp-cli -g && \
    gulp --help

WORKDIR /opt/app

EXPOSE 8877
EXPOSE 3001

VOLUME ["/opt/app"]

#CMD ["gulp", "serve"]

#docker run -p 8877:8877 -p 3001:3001 --name nodeapp -i -t --rm -v ~/workspace/project-x/node:/opt/app gulp bash




