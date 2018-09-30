FROM php:7.0

RUN apt-get update && \
    apt-get install -y freetds-dev wget git

RUN ln -s /usr/lib/x86_64-linux-gnu/libsybdb.a /usr/lib/ && \
    docker-php-ext-install pdo_dblib

WORKDIR /data/

CMD ['php']