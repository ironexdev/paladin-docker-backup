FROM mongo:5.0.3

ARG DOCKER_IMAGE_CONTEXT_PATH

RUN mkhomedir_helper mongodb

COPY $DOCKER_IMAGE_CONTEXT_PATH/mongo/init.js /docker-entrypoint-initdb.d/

USER mongodb

EXPOSE 27017