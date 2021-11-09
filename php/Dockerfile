#  fpm es un servicio que escucha en port 9000, que recibe php para ser interpretado
# lo configuramos en conf apache, todo lo que tenga php lo pasas a el container con php
FROM php:8.1.0RC5-fpm-alpine

#  -Al usar alpine no tenemos apt-get de Debian
# RUN apt-get update \
#     && apt-get upgrade -y

RUN apk add --no-cache nginx

# módulo mysqli
RUN docker-php-ext-install mysqli