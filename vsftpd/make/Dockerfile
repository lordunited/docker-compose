FROM centos:7
MAINTAINER infra
ARG version=1.0
LABEL version="1.0"
ENV vsftpd_dir=/home/
ENV vsftpd_conf=/etc/vsftpd
RUN yum install -y vim telnet wget vsftpd 
USER root
COPY . ${vsftpd_conf}
ENTRYPOINT ["/bin/bash"]
EXPOSE 20 21
