FROM centos:6
MAINTAINER Meaghan Johnson <mejohn10@ncsu.edu>

RUN yum -y update && yum groupinstall -y "Development Tools"
RUN rpm -Uvh http://repos.mesosphere.io/el/6/noarch/RPMS/mesosphere-el-repo-6-2.noarch.rpm
RUN yum -y install mesos
