FROM alpine:latest
RUN apk update && apk upgrade && apk add apache2 && rm -rf /etc/apache2/conf.d/000-default.conf
COPY /Apache/000-default.conf /etc/apache2/conf.d/
EXPOSE 80
CMD [“/usr/sbin/httpd”, “-D”, “FOREGROUND”]
