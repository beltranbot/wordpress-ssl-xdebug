FROM wordpress:5.7.1-apache

RUN a2enmod ssl

RUN service apache2 restart

COPY ./apache/default-ssl.conf /etc/apache2/sites-enabled/default-ssl.conf

COPY ./certs/docker.crt /etc/ssl/docker.crt

COPY ./certs/docker.key /etc/ssl/docker.key

EXPOSE 443
