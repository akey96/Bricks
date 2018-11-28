FROM centos:7

LABEL version=1.0

# RUN \
#   yum -y install \
#     epel-release \
#     yum-utilssudo \
#     http://rpms.remirepo.net/enterprise/remi-release-7.rpm

# RUN yum-config-manager --enable remi-php72

RUN \
  yum -y install \
    epel-release \
    yum-utilssudo \
    http://rpms.remirepo.net/enterprise/remi-release-7.rpm


RUN yum-config-manager --enable remi-php56

RUN \
  yum -y install \
    php \
    php-mcrypt \
    php-cli \
    php-gd \
    php-curl \
    php-mysql \
    php-ldap \
    php-zip \
    php-fileinfo

RUN yum -y install httpd

CMD apachectl -DFOREGROUND