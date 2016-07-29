FROM daocloud.io/library/centos:6

RUN yum install -y \
java-1.7.0-openjdk.x86_64 \
openssh-server

RUN curl \
http://d3kbcqa49mib13.cloudfront.net/spark-2.0.0-bin-hadoop2.7.tgz \
| tar -xzC /opt
RUN ln -s /opt/spark-2.0.0-bin-hadoop2.7 /opt/spark

ENV SPARK_HOME /opt/spark
ENV PATH $SPARK_HOME:$PATH
