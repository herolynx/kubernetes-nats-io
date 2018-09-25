# nats-io

DevOps prepared for NATS.

## Server

Basic NATS server with `Prometheus` used for monitoring and exporting metrics.

1) Create NATS cluster

```bash
kubect apply -f nats-io/
```

## Streaming

[NATS streaming](https://github.com/nats-io/go-nats-streaming) is prepared since it provides:

* Log based persistence

* At-Least-Once Delivery model, giving reliable message delivery

* Rate matched on a per subscription basis

* Replay/Restart

* Last Value Semantics

1) Create NATS streaming cluster

```bash
kubect apply -f nats-streaming/
```

## Docs

* [Nats operator](https://github.com/nats-io/nats-operator)

* [Kubernetes NATS cluster](https://github.com/pires/kubernetes-nats-cluster)