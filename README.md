# bosh-redis

A [*Redis*](https://redis.io/) release for Cloud Foundry

## Features

- High availability by [*Redis Sentinel*](https://redis.io/topics/sentinel)
- [*Redis cluster*](https://redis.io/topics/cluster-spec) with high availability
- Multi-zone for high availability by Redis Sentinel and Redis cluster with high availability,
- Monitoring by [*Prometheus*](https://prometheus.io/)/[*Grafana*](https://grafana.com/)

## TODO

- Tests for [*persistence*](https://redis.io/topics/persistence)
- Backup/restore
- Logging

## Packages versions summary

- Redis 5.0.3
- [*redis_exporter*](https://github.com/oliver006/redis_exporter/releases) 0.30.0

## Usage

- Clone the repository:
```
git clone https://github.com/orange-cloudfoundry/redis-orange
```
- Create release
```
bosh create-release
```
- Upload release
```
bosh upload-release
```

**Note**: For security purposes, we use [*CredHub*](https://docs.cloudfoundry.org/credhub/)  for passwords and to obfuscate some Redis admin commands.
