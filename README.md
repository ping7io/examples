# 💡 Integration Examples

This repository contains example integrations of the [ping7.io](https://ping7.io) SaaS for [Prometheus](https://prometheus.io/).

## Available Exporters

Under the hood we are utilizing

### Blackbox Exporter

* https://github.com/prometheus/blackbox_exporter

### SSL Labs Exporter

* https://github.com/anas-aso/ssllabs_exporter

### SSL Exporter

* https://github.com/ribbybibby/ssl_exporter

## Running this example project

1. 🐳 To run the example project, you need to have [Docker](https://www.docker.com/products/docker-desktop) installed
1. 📦 Clone this project or download and unzip the sources
1. 🔥 Register with [ping7.io](https://ping7.io/signup) and activate your API key
1. 🔐 Replace all `YOUR_API_KEY` placeholder in the `prometheus.yml` with your ping7.io API key
1. 🤖 Use `docker compose` to launch a local Prometheus instance

```shell
$ docker compose up
```

Upon start, you can:

* view the [configured Prometheus targets](http://localhost:9090/targets)
* query the [gathered metrics](http://localhost:9090/graph?g0.expr=probe_success&g0.tab=1&g0.stacked=0&g0.show_exemplars=0&g0.range_input=1h)
* analyze the [alarming rules](http://localhost:9090/alerts)

## License

This project is licensed under the [MIT License](LICENSE).
