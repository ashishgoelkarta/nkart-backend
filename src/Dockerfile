# Use the official Elasticsearch image from Docker Hub
FROM docker.elastic.co/elasticsearch/elasticsearch:8.6.0
 
# Set environment variables for Elasticsearch
ENV discovery.type=single-node
ENV ES_JAVA_OPTS="-Xms1g -Xmx1g"
 
# Enable security features and set password for 'elastic' user
ENV ELASTIC_PASSWORD=asdf
 
# Expose the default Elasticsearch port
EXPOSE 9200 9300
