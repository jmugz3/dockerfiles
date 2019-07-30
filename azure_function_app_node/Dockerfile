FROM node:10.14.1-alpine

RUN mkdir -p /home/src/node_modules && chown -R node:node /home/src
WORKDIR /home/src

USER node
# COPY --chown=node:node . .

COPY package*.json ./

# RUN npm install azure-functions-core-tools

RUN echo "Running npm: $(npm -v)" \
    && echo "Running node: $(node -v)" \
    && echo "Working Directory: $(pwd)" \
    && echo "packages: $(npm ls --depth 0)" \
    && echo "Directory: $(ls -a)" \
    && echo "Directory: $(ls -a node_modules/)" \
    && echo "Running az-func-tools version: $(func -v)"

