# Rabbit & Redis
Simple rabbit node and Redis cluster. Rabbit with mqtt plugin enabled for test environment.
- http://localhost:15672, rabbitmq web
- 5672: amqp protocol
- 1883: mqtt protocol
- 6379: redis protocol

- guest/guest: default user/password for rabbitmq
- redis-cluster without security

## Start up
- Normal start up
```sh
docker-compose -f rabbitmq-redis-dc.yml up -d
```
- Stop
```sh
docker-compose -f rabbitmq-redis-dc.yml down
```
- Start & rebuild
```sh
docker-compose -f rabbitmq-redis-dc.yml up -d --build
```