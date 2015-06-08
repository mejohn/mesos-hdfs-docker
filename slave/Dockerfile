FROM mejohn/mesos
MAINTAINER Meaghan Johnson <mejohn10@ncsu.edu>

RUN yum -y update && yum -y install wget tar java-1.7.0-openjdk
RUN wget https://archive.apache.org/dist/hadoop/core/hadoop-2.4.1/hadoop-2.4.1.tar.gz
RUN tar zxvf hadoop-2.4.1.tar.gz && mv hadoop-2.4.1 /usr/local/hadoop
ADD core-site.xml /usr/local/hadoop/etc/hadoop/core-site.xml
ENTRYPOINT mesos-slave
EXPOSE 5051 
