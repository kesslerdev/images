FROM nginx

COPY --chown=www-data:www-data conf /etc/nginx/conf.d/
COPY --chown=www-data:www-data nginx.conf /etc/nginx/nginx.conf

COPY --chown=www-data:www-data entrypoint.sh /entrypoint.sh

ENTRYPOINT /entrypoint.sh
