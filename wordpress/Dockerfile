FROM ubuntu:14.04
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get install -y curl
RUN curl https://wordpress.org/latest.tar.gz --insecure | tar -xvzf -
ADD router.php /wordpress/router.php 
ADD wp-config.php /wordpress/wp-config.php 
RUN chown -R root:root /wordpress
VOLUME /wordpress
