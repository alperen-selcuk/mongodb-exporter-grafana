# mongodb-exporter-grafana

for this configuration you can collect mongodb metric from mongodb server to grafana.

## mongodb exporter

first you need to install mongodb exporter binary then run mongodb exporter with mongo connection string
you can find offical github page for your platform.

https://github.com/percona/mongodb_exporter 

after the binary installation run command like below. 

```
mongodb_exporter --mongodb.uri=mongodb://adminuser:password@mongodbip:port" --web.listen-address=:9001 --collect-all
```

## prometheus 

then you need to collect metric with prometheus. you can install with offical page

https://github.com/prometheus/prometheus


