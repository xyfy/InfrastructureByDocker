# Infrastructure Provided By Docker For Local dev

Infrastructure Provided By Docker ，Include RabbitMQ、Redis、Mongodb、mongo-express、ELK。

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

> support `Redis`,`elasticsearch`,`mongodb`,`rabbitmq`、`kibana`、`logstash`

## Tips

RabbitMQ use TZ  `Asia/Shanghai`
