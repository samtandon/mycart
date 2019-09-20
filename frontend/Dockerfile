# This is a dockerfile for mycart's MS frontend layer
#CENTOS 7.2
#Update all your existing packages: yum -y update
#Install apache: yum -y install httpd
#Install Php : yum -y install php php-gd
#copy code from frontend/code to /var/www/html
#run apache on port 80

#ADD copies folder contents, will also extract zip files- .zip and .tgz. it can even take from URL. COPY will copy folder alongwith contents

FROM centos:7
MAINTAINER samtandon2588@gmail.com
RUN yum -y update
RUN yum -y install httpd
RUN yum -y install php php-gd
ADD code /var/www/html
ENV BACKENDLB=test
EXPOSE 80
CMD ["httpd", "-D", "FOREGROUND"]