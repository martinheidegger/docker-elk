FROM elasticsearch:latest
LABEL version="1.0"
RUN plugin install elasticsearch/license/latest
RUN plugin install elasticsearch/shield/latest
COPY shield /etc/elasticsearch/shield
COPY shield /usr/share/elasticsearch/config/shield
