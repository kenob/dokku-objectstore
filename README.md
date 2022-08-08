# [WIP] dokku minio

S3-compatible object storage based on minio [minio](https://min.io)

## Requirements

- dokku 0.19.x+
- docker 1.8.x

## Installation

```shell
# on 0.19.x+
sudo dokku plugin:install https://github.com/kenob/dokku-minio.git minio
```

## Commands

```
minio:create <service>                      # create a minio service
minio:destroy <service>                     # destroy a minio service
minio:link <service> <app>                  
minio:enter <service>
minio:exists <service>
minio:start <service>                       # start minio service container
minio:restart <service>                     # graceful shutdown and restart of the minio service container
minio:stop <service>                        # graceful shutdown of the minio service container
```
