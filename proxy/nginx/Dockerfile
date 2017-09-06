FROM nginx:latest

MAINTAINER Hierony Manurung (hieronymilanisti09@gmail.com)

RUN apt-get update \
        && apt-get install openssl --no-install-recommends --no-install-suggests -y \
        && rm -fr /var/lib/apt/lists/*
