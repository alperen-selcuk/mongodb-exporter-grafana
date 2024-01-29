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

## grafana

final step you need to create datasource on grafana.  doesnt matter where is grafana working, docker, server or kubernetes. same UI same configuration

add datasource with prometheus port

<img width="940" alt="image" src="https://github.com/alperen-selcuk/mongodb-exporter-grafana/assets/78741582/236c1df2-6365-4577-809a-22bf11a7aec1">

after the adding data source you need to import dashboard
i prefer this one id 16490 
you can find all metric for mongodb.

