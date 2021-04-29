# ITHX-Exporter
A library that connects the ITHX Omega sensors to Prometheus

```
docker run -d -p 9090:9090 prom/prometheus -v /Users/steven/Development/OSUSensors/:config --config.file=/config/prometheus.yml  
docker run -d -p 9115:9115 --name blackbox_exporter -v `pwd`/config prom/blackbox-exporter --config.file=/Users/steven/Development/OSUSensors/blackbox.yml
```
