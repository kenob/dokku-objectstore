# [WIP] dokku objectstore

S3-compatible object storage backed by [minio](https://min.io). Implementation inspired by [dokku-postgres](https://github.com/dokku/dokku-postgres)

## Requirements

- dokku 0.19.x+
- docker 1.8.x

## Installation

```shell
# on 0.19.x+
sudo dokku plugin:install https://github.com/kenob/dokku-objectstore.git objectstore
```

## Commands

```
objectstore:create <service>                      # create an objectstore service
objectstore:destroy <service>                     # destroy an objectstore service
objectstore:clone <service>                       # clone a service
objectstore:connect <service>                     # connect to an objectstore service
objectstore:link <service> <app>                  
objectstore:enter <service>
objectstore:exists <service>
objectstore:start <service>                       # start an objectstore service container
objectstore:restart <service>                     # graceful shutdown and restart of the objectstore service container
objectstore:stop <service>                        # graceful shutdown of the objectstore service container
```
