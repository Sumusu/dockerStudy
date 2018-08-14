FROM centos:6.7

RUN touch /var/lib/rpm/*
RUN yum -y update && yum -y install wget && yum clean all
RUN yum -y install httpd | true && yum clean all

EXPOSE 80

ENTRYPOINT [ "/usr/sbin/httpd" ]

CMD ["-D","FOREGROUND"]