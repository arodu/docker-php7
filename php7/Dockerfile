FROM webdevops/php-apache-dev:7.4

RUN apt update

RUN apt install -y apt-utils sendmail mariadb-client \
  pngquant unzip zip libpng-dev libmcrypt-dev git curl libicu-dev \
  libxml2-dev libssl-dev sqlite libpq-dev postgresql-client

RUN apt install -y libjpeg-dev
RUN apt install -y libssh2-1 

RUN docker-php-ext-configure gd --with-jpeg

RUN docker-php-ext-install gd intl pdo pdo_mysql pdo_pgsql pgsql mysqli
