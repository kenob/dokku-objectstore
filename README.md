# [WIP] dokku objectstore

S3-compatible object storage backed by [minio](https://min.io). Implementation based on [dokku-postgres](https://github.com/dokku/dokku-postgres)

## Requirements

- dokku 0.19.x+
- docker 1.8.x

## Installation

```shell
# on 0.19.x+
sudo dokku plugin:install https://github.com/kenob/dokku-objectstore.git minio
```

## Commands

```
objectstore:create <service>                      # create a minio service
objectstore:destroy <service>                     # destroy a minio service
objectstore:link <service> <app>                  
objectstore:enter <service>
objectstore:exists <service>
objectstore:start <service>                       # start minio service container
objectstore:restart <service>                     # graceful shutdown and restart of the minio service container
objectstore:stop <service>                        # graceful shutdown of the minio service container
```
