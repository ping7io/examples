# 💡 ping7.io integration examples

This repository contains example integrations for the [ping7.io](https://ping7.io)
SaaS for managed Exporters for [Prometheus](https://prometheus.io/).

## Prerequisites

Register with [ping7.io](https://ping7.io/signup) and acquire an API token.

## Example integations

This project contains the following example integrations.

### 🐳 Docker

[Launches a local Prometheus via Docker that checks statically configured
websites via the ping7.io API.](docker/). This example is the easiest first
time starting point.

### 🎡 Kubernetes

[Launches a local Minikube cluster and checks all Ingresses configured in
the cluster via the ping7.io API.](kubernetes/). When Kubernetes is your
primary compute source, this integration adapts to any change made to your
Ingresses.

## Further reading

For detailed configuration options, head over to
[`docs.ping7.io`](https://docs.ping7.io)

## License

This project is licensed under the [MIT License](LICENSE).
