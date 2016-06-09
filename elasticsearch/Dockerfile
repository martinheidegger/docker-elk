FROM elasticsearch:latest
LABEL version="1.0"
RUN plugin install elasticsearch/license/latest
RUN plugin install elasticsearch/shield/latest
COPY shield /usr/share/elasticsearch/config/shield
RUN rm -r /etc/elasticsearch/shield
RUN ln -s /usr/share/elasticsearch/config/shield /etc/elasticsearch/shield
RUN chown -R elasticsearch:elasticsearch /usr/share/elasticsearch/config/shield
