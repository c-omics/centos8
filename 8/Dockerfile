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
                   git     \
                   gcc     \
                   gcc-c++ \ 
                   make    \
                   net-tools \
                   which && \
    yum clean all && \
    rm -rf /var/cache/yum 

COPY user_entrypoint.sh /usr/local/bin/user_entrypoint.sh
ENTRYPOINT ["/usr/local/bin/user_entrypoint.sh"]
