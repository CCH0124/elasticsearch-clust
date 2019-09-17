# elasticsearch-clust

## import json file
```shell
$ wget https://download.elastic.co/demos/kibana/gettingstarted/logs.jsonl.gz
$ gunzip logs.jsonl.gz
$ curl -H 'Content-Type: application/x-ndjson' -XPOST 'localhost:9200/_bulk?pretty' --data-binary @logs.jsonl
```
