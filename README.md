# Homeserver monitoring stack
My personal exporter stack to push local metrics to Grafana Cloud

## What does it contain?
* Prometheus
* Promtail
* syslog-ng
* apcupsd exporter
* Ping exporter
* Blackbox exporter
* Node exporter

## Requirements
* Linux host
* Docker 20.10+

## How to run
1. You need to have installed loki plugin for docker
```
docker plugin install grafana/loki-docker-driver:latest --alias loki --grant-all-permissions
```
2. Enter Loki push URL in `.env`
3. `docker-compose up -d`

