# Running

The nats-server has many command line options. To get started, you don't have to specify anything. In the absence of any flags, the NATS server will start listening for NATS client connections on port 4222. By default, security is disabled.

## Standalone

When the server starts it will print some information including where the server is listening for client connections:

```text
> nats-server
[9318] 2020/02/06 14:06:08.220885 [INF] Starting nats-server version 2.1.4
[9318] 2020/02/06 14:06:08.221099 [INF] Git commit [fb009af]
[9318] 2020/02/06 14:06:08.221466 [INF] Listening for client connections on 0.0.0.0:4222
[9318] 2020/02/06 14:06:08.221476 [INF] Server id is NAINBEK336OZMOZUBNOFCJWG4Q2XNFEROWLF6FQWOGM4CBLI5Y6G33NW
[9318] 2020/02/06 14:06:08.221478 [INF] Server is ready
...
```

## Docker

If you are running your NATS server in a docker container:

```text
docker run -p 4222:4222 -ti nats:latest
[1] 2020/02/06 19:04:56.020658 [INF] Starting nats-server version 2.1.4
[1] 2020/02/06 19:04:56.020712 [INF] Git commit [fb009af]
[1] 2020/02/06 19:04:56.020833 [INF] Starting http monitor on 0.0.0.0:8222
[1] 2020/02/06 19:04:56.020897 [INF] Listening for client connections on 0.0.0.0:4222
[1] 2020/02/06 19:04:56.020919 [INF] Server id is NBSNFHIXGTZJ4OCMHU52UGVOLCJEKYTYEAFMABDJUAKZUQE2ULXBQGHX
[1] 2020/02/06 19:04:56.020923 [INF] Server is ready
[1] 2020/02/06 19:04:56.021174 [INF] Listening for route connections on 0.0.0.0:6222
...
```

More information on [containerized NATS is available here](../nats_docker/README.md).

