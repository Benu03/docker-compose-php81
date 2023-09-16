FROM phpdockerio/php:8.1-fpm
WORKDIR "/application"

RUN apt-get update
RUN apt-get install -y libpq-dev 
RUN apt-get install -y libzip-dev
RUN apt-get install -y snmp-mibs-downloader
RUN apt-get install -y iputils-ping
RUN apt-get install -y net-tools
RUN apt-get install -y git

RUN apt-get update; \
    apt-get -y --no-install-recommends install \
    php8.1-mongodb \ 
    php8.1-oauth \ 
    php8.1-odbc \ 
    php8.1-dev \
    php8.1-xml \
    php8.1-pgsql; \
    apt-get clean; \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*
# RUN pecl install sqlsrv
# RUN pecl install pdo_sqlsrv
