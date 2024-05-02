FROM centos:7
RUN yum install httpd -y
RUN mkdir -p /var/www/html/home/
WORKDIR /var/www/html/
COPY index.html home/index.html
COPY style.css home/style.css
RUN echo "ServerName localhost" >> /etc/httpd/conf/httpd.conf
EXPOSE 80
CMD ["httpd", "-D", "FOREGROUND"]