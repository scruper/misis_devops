FROM alpine:3
RUN apk add --update nginx && rm -rf /var/cache/apk/*

COPY config/default.conf /etc/nginx/http.d/default.conf
COPY static /var/www/hello_world

CMD ["nginx", "-g", "daemon off;"]