# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash:5.6.3

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
RUN logstash-plugin install logstash-input-beats && \
    logstash-plugin install logstash-filter-csv && \
    logstash-plugin install logstash-filter-grok && \
    logstash-plugin install logstash-output-elasticsearch && \
    logstash-plugin install logstash-codec-rubydebug
