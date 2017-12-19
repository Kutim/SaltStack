FROM centos:7

LABEL maintainer="kutim@1252900197@qq.com"


RUN yum install -y https://repo.saltstack.com/yum/redhat/salt-repo-latest-2.el7.noarch.rpm && \
    yum clean expire-cache && \
    yum install -y salt-master

RUN yum install -y python-setuptools && \
    easy_install supervisor

RUN mkdir -p /var/log/supervisor
ADD supervisord.conf /etc/supervisord.conf
ADD accept.sh ./

CMD ["/usr/bin/supervisord"]
