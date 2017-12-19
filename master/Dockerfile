FROM centos:7

LABEL maintainer="kutim@1252900197@qq.com"


RUN yum install -y https://repo.saltstack.com/yum/redhat/salt-repo-latest-2.el7.noarch.rpm && \
    yum clean expire-cache && \
    yum install -y salt-master
