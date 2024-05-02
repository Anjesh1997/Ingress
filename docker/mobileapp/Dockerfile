FROM centos:7
RUN yum install httpd -y
RUN mkdir -p var/www/html/mobile/
WORKDIR /var/www/html/
COPY index.html mobile/index.html
EXPOSE 80
CMD ["httpd","-D","FOREGROUND"]