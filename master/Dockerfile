FROM mesosphere/mesos-master:0.22.1-1.0.ubuntu1404
MAINTAINER Meaghan Johnson <mejohn10@ncsu.edu>

RUN apt-get update && apt-get -y install wget
RUN wget https://archive.apache.org/dist/hadoop/core/hadoop-2.4.1/hadoop-2.4.1.tar.gz
RUN tar zxvf hadoop-2.4.1.tar.gz && mv hadoop-2.4.1 /usr/local/hadoop
ADD core-site.xml /usr/local/hadoop/etc/hadoop/core-site.xml

CMD ["--registry=in_memory"]
ENTRYPOINT ["mesos-master"]

EXPOSE 5050 
