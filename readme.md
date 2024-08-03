# Infrastructure Provided By Docker For Local dev

Infrastructure Provided By Docker ，Include grafana、 prometheus、 RabbitMQ、 Redis、 SqlServer、 ELK ~~、Mongodb、mongo-express~~。

Each of the services has none password、default port.

## Usage

start all services

``` sh
docker-compose -f docker-compose.infrastructure.yml -f docker-compose.infrastructure.override.yml up -d
```

stop all

```sh
docker-compose -f docker-compose.infrastructure.yml -f docker-compose.infrastructure.override.yml down
```

start special services, such as `Redis`

``` sh
docker-compose -f docker-compose.infrastructure.yml -f docker-compose.infrastructure.override.yml up -d redis rabbitmq
```

> support `Redis`,`elasticsearch`,`grafana`,`rabbitmq`、`kibana`、`prometheus`、`SqlServer`

## Tips

RabbitMQ use TZ  `Asia/Shanghai`
