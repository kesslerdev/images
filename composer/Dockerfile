FROM composer:latest

RUN composer global require hirak/prestissimo && chmod 777 -R /tmp

RUN ssh-keyscan -H github.com >> /etc/ssh/ssh_known_hosts
