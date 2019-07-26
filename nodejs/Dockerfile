FROM ubuntu

RUN apt-get update \
        && wget http://nodejs.org/dist/node-latest.tar.gz \
        && tar xvzf node-latest.tar.gz \
        && cd node-v* \
        && ./configure \
        && echo "Using node $(node --version)"
