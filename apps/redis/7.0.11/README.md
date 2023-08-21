# Redis

> The open source, in-memory data store used by millions of developers as a database, cache, streaming engine, and message broker.

This version of Redis creates a single redis node with persistent storage. Make sure to configure redis appropriately with your persistence preferences using the official documentation.

After deploying the application, you will be able to connect to redis using *redis-server* as the target host. The client application must be deployed on the same environment to have access to redis.

## Manual connection

To execute commands directly on the redis instance, you can connect to it using the *kubectl* tool for kubernetes following the next steps:

1. Login into the playground from the CLI

```bash
playground login
```

2. Open a shell in the target deployment and execute [redis-cli](https://redis.io/docs/manual/cli/)

```bash
$ kubectl --kubeconfig ~/.napptive/default/napptive-kubeconfig exec -it deploy/redis-server -- redis-cli
127.0.0.1:6379> PING
PONG
127.0.0.1:6379> exit
```
