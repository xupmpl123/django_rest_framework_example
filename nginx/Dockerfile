FROM nginx:latest

RUN rm /etc/nginx/conf.d/default.conf

COPY ./nginx.conf /etc/nginx/conf.d/

RUN mkdir -p /var/www/media
RUN mkdir -p /var/www/static

WORKDIR /var/www/media
RUN chown -R nginx:nginx /var/www/media

WORKDIR /var/www/static
RUN chown -R nginx:nginx /var/www/static