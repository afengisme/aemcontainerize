FROM httpd:2.4

ADD install /install

WORKDIR /install

RUN cp -f dispatcher-apache2.4-4.2.3.so /usr/local/apache2/modules/; \
    ln -s /usr/local/apache2/modules/dispatcher-apache2.4-4.2.3.so /usr/local/apache2/modules/mod_dispatcher.so; \
    cp -f conf/dispatcher.any /usr/local/apache2/conf/; \
    mkdir -p /usr/apachecache/docs; \
    cp -f httpd.conf /usr/local/apache2/conf/;


EXPOSE 80
CMD ["httpd-foreground"]
