# Jstatbeat

Jstatbeat is the [Beat](https://www.elastic.co/products/beats) used for
JVM GC monitoring. It reads jstat results and indexes them in Elasticsearch.

## Elasticsearch template

To apply jstatbeat template:

    curl -XPUT 'http://localhost:9200/_template/jstatbeat' -d@jstatbeat.template.json

## Kibana dashboard

Import [dashboard.json](https://github.com/cero-t/jstatbeat/blob/master/etc/dashboard.json) into kibana to create dashboards for jstatbeat.
