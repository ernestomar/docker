FROM ubuntu:16.04
LABEL maintainer="ernestomar@gmail.com"
ENV DEBIAN_FRONTEND noninteractive

VOLUME ["/var/www/html"]

RUN apt-get update && \
    apt-get -y upgrade 
RUN apt-get install -y apache2
RUN	apt-get install -y php7.0 \
	 		libapache2-mod-php7.0 \ 
			php7.0-cli \
			php7.0-common \
			php7.0-mbstring \
			php7.0-gd \
			php7.0-intl \
			php7.0-xml \
			php7.0-mysql \
			php7.0-mcrypt \
			php7.0-zip \
			php7.0-pgsql 

EXPOSE 80

ENTRYPOINT [ "apachectl", "-DFOREGROUND"  ]
# COPY config/php.ini /usr/local/etc/php/
# COPY src/ /var/www/html/

