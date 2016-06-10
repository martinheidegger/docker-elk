FROM elasticsearch:latest
LABEL version="1.0"
RUN plugin install elasticsearch/license/latest
RUN plugin install elasticsearch/shield/latest
RUN rm -r /etc/elasticsearch/shield
COPY shield /usr/share/elasticsearch/config/shield
RUN ln -s /usr/share/elasticsearch/config/shield /etc/elasticsearch/shield
RUN chown -R elasticsearch:elasticsearch /usr/share/elasticsearch/config/shield
