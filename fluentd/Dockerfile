FROM fluent/fluentd

RUN gem install fluent-plugin-elasticsearch -v 1.18.0 && \
	gem sources --clear-all && \
	rm -rf \
    /var/cache/apk/* \
    /tmp/* \
    /var/tmp/* \
    /usr/lib/ruby/gems/*/cache/* \
    /home/fluent/.gem/ruby/*/cache/*.gem

COPY baizley.conf /fluentd/etc/baizley.conf
