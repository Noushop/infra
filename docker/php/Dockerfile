FROM chialab/php-dev:7.4-fpm


RUN rm -rf /var/lib/apt/lists/*
RUN apt-get update -o Acquire::CompressionTypes::Order::=gz
RUN apt-get update -y && ACCEPT_EULA=Y apt-get upgrade -y && apt-get install -y git

# Install Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
RUN composer config --global --auth gitlab-token.gitlab.com Up5ZXTzF9yeVzfCxpetz

WORKDIR /var/www/vhosts