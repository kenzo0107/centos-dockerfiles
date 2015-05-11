FROM centos:centos6

MAINTAINER Kenzo Tanaka <kenzo.tanaka0107@gmail.com>

RUN yum -y update; yum clean all
RUN yum -y install httpd; yum clean all
RUN echo "Working" >> /var/www/html/index.html

EXPOSE 80

ADD run-httpd.sh /run-httpd.sh
RUN chmod -v +x /run-httpd.sh

CMD ["/run-httpd.sh"]
