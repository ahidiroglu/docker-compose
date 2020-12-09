FROM nginx:1.11

COPY ./files/ /etc/ssl/certs/nginx/
COPY ./nginx.conf /etc/nginx/conf.d/default.conf

RUN apt-get update -y && apt-get install -y nginx
EXPOSE 80
EXPOSE 443
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]