FROM n0ts/amazonlinux

MAINTAINER Naoya Nakazawa <naoya.n@gmail.com>

COPY nginx.repo /etc/yum.repos.d/

RUN set -x \
    && yum install -y nginx \
    && nginx -V \
    && ln -sf /dev/stdout /var/log/nginx/access.log \
    && ln -sf /dev/stderr /var/log/nginx/error.log

COPY nginx.conf /etc/nginx/
COPY status.conf /etc/nginx/conf.d/
COPY site.conf.orig /etc/nginx/conf.d/
COPY index.html /usr/share/nginx/html/

EXPOSE 80

STOPSIGNAL SIGTERM

CMD ["nginx", "-g", "daemon off;"]
