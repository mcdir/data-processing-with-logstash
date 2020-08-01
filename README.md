This repository contains all of the configuration files used within the 
[Data Processing with Logstash course](https://l.codingexplained.com/course/logstash?src=github).

# prepare

    cp -r ./data /tmp/

# test for Basics/file-output.conf

```bash
curl --request PUT \
  --url http://127.0.0.1:8080/ \
  --header 'cache-control: no-cache' \
  --header 'content-type: application/json' \
  --data '{"quantity": "1000000" }'
```

# clean up cache

    rm /opt/logstash-7.4.0/data/plugins/inputs/file/.sincedb_*