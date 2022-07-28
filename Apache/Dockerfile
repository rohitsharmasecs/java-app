FROM alpine:latest
RUN apk update && apk upgrade && apk add apache2 && rm -rf /etc/apache2/sites-available/000-default.conf
COPY /Apache/000-default.conf /etc/apache2/sites-available/
EXPOSE 80
CMD [“httpd”, “-D”, “FOREGROUND”]
