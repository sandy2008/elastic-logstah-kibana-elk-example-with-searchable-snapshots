# elastic-logstah-kibana-elk-example-with-searchable-snapshots
The Elastic stack (ELK) &amp; tests with searchable snapshots powered by Docker Compose.

## Getting Started
```
ELK_VERSION=7.10.1 docker-compose build
ELK_VERSION=7.10.1 docker-compose up
```
## S3 Repo Creation
```
http://127.0.0.1:9200/_snapshot/s3
```
- Body
```
{ 
    "type": "s3", 
    "settings": { 
        "bucket": "data", 
        "region": "us-east-1", 
        "endpoint": "http://172.25.0.2:9000",  
        "access_key": "user", 
        "secret_key": "freehongkong8964", 
        "protocol": "http" 
    }
 }
 ```

 ## Filesystem Repo Creation
 ```
{
  "type": "fs",
  "settings": {
    "location": "/var/tmp/es",
    "compress": true
  }
}
 ```