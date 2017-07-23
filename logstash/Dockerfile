# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash:5.5.0

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json

ADD ./conf/logstash.yml /usr/share/logstash/config/
ADD ./conf/logstash.conf /usr/share/logstash/pipeline/
