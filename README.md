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
objectstore:connect <service>                     # connect to an objectstore service using the `mc` tool
objectstore:link <service> <app>                  # link a service to an app
objectstore:unlink <service> <app>                # unlink a service from an app
objectstore:info <service>                        # display information about a service
objectstore:logs <service>                        # view logs for the service container
objectstore:expose <service> [PORT]               # make the service accessible from outside the container on PORT
objectstore:unexpose <service>                    # unexpose the service
objectstore:enter <service>                       # open a shell session inside the service container
objectstore:exists <service>                      # check if a service exists
objectstore:list                                  # display a list of services
objectstore:start <service>                       # start an objectstore service container
objectstore:restart <service>                     # graceful shutdown and restart of the objectstore service container
objectstore:stop <service>                        # graceful shutdown of the objectstore service container
```
