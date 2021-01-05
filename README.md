# elastic-logstah-kibana-elk-example-with-searchable-snapshots
The Elastic stack (ELK) &amp; tests with searchable snapshots powered by Docker Compose.

## Getting Started
```
ELK_VERSION=7.10.1 docker-compose build
ELK_VERSION=7.10.1 docker-compose up
```
## S3 Repo Creation
```
http://127.0.0.1:9200/_snapshot/my_minio_repository
```