FROM centos:7

RUN yum -y install wget 

RUN cd /tmp/ && wget --quiet https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-5.5.0-linux-x86_64.tar.gz

RUN tar xzf /tmp/filebeat-5.5.0-linux-x86_64.tar.gz -C /opt/

RUN mv /opt/filebeat-5.5.0-linux-x86_64 /opt/filebeat

RUN rm -rf /tmp/filebeat-5.5.0-linux-x86_64.tar.gz 

ADD ./logs/ /opt/logs/

ADD ./conf/filebeat.yml /opt/filebeat/filebeat.yml

CMD /opt/filebeat/filebeat -e -v -c /opt/filebeat/filebeat.yml
