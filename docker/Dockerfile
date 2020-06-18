FROM docker.elastic.co/elasticsearch/elasticsearch:7.2.0

COPY ik /usr/share/elasticsearch/plugins/ik
COPY elasticsearch.yml /usr/share/elasticsearch/config/elasticsearch.yml

USER 10000