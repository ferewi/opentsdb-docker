### Supported tags and respective ```Dockerfile``` links
The tags have the following format: ```OpenTSDBVersion_HBaseVersion```
* [```2.3_1.1.3```, (2.3_1.1.3/Dockerfile)](https://github.com/jimtonic/opentsdb-docker/blob/2.3_1.1.3/Dockerfile)
* [```2.3_1.2.4```,```latest```, (2.3_1.2.4/Dockerfile)](https://github.com/jimtonic/opentsdb-docker/blob/2.3_1.2.4/Dockerfile)

## How To Use

### 1. Run the image

```
docker run -d --name some_opentsdb jimtonic/opentsdb
```

Exposed Ports:
* 4242  - OpenTSDB REST API
* 16010 - HBase Master web UI at :16010/master-status;  ZK at :16010/zk.jsp

### 2. Bind a data directory
```
docker run -d --name some_opentsdb -v your_local_dir:/data/hbase jimtonic/opentsdb
```

