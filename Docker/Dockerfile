# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
#             Best practices for writing Dockerfiles
https://docs.docker.com/develop/develop-images/dockerfile_best-practices/
# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# Dockefile to build Docker Image of Apache WebServer running on Ubuntu
# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

FROM ubuntu:16.04

RUN apt-get -y update
RUN apt-get -y install apache2

RUN echo 'Hello World from Docker!' > /var/www/html/index.html


CMD ["/usr/sbin/apache2ctl", "-D","FOREGROUND"]
EXPOSE 80
# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# Dockefile to build Docker Image of Apache WebServer running on AmazonLinux 
# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

FROM amazonlinux

RUN yum -y update
RUN yum -y install httpd

RUN echo 'Hello World from Docker!' > /var/www/html/index.html
CMD ["/usr/sbin/httpd","-D","FOREGROUND"]

EXPOSE 80
