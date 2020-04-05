FROM centos:8
MAINTAINER Ian Merrick <MerrickI@Cardiff.ac.uk>

##############################################################
# Software:             -
# Software Version:     -
# Software Website:     -
# Description:          Base Centos8 with ansible/epel/gcc/git
##############################################################

RUN dnf update -y && \ 
    dnf install -y epel-release && \
    dnf install -y ansible \
                   bzip2   \
                   git     \
                   gcc     \
                   gcc-c++ \ 
                   make    \
                   net-tools \
                   which && \
    yum clean all && \
    rm -rf /var/cache/yum 

WORKDIR /home
