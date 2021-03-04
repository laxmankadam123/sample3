FROM centos:7


RUN yum  update -y

RUN yum  install httpd* -y


RUN rpm -Uvh https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm


RUN yum  install php php-mysql php-cgi php-cli php-gd -y


COPY index.php /var/www/html/


EXPOSE 80

CMD ["/usr/sbin/httpd","-D","FOREGROUND"]
