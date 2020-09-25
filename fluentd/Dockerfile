FROM fluent/fluentd:v1.11.2-1.0

USER root

RUN gem install fluent-plugin-elasticsearch -v 1.18.0 && \
    gem install fluent-plugin-detect-exceptions && \
    gem install fluent-plugin-route && \
	gem sources --clear-all && \
	rm -rf \
    /var/cache/apk/* \
    /tmp/* \
    /var/tmp/* \
    /usr/lib/ruby/gems/*/cache/* \
    /home/fluent/.gem/ruby/*/cache/*.gem

COPY baizley.conf /fluentd/etc/baizley.conf
