# docker-compose-test

## Containers

```
                      _ web1
                     /
nginx_loadbalancer -> 
                     \_ web2
                     
mysql_percona
```

## Create config.env for storing environment variables and secrets

```
$ car PASSWORD=password > config.env
```

## Run

```
$ docker-compose up --env-file config.env
```
