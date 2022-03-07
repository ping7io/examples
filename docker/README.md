# 💡 Integration Examples

This repository contains example integrations for the [ping7.io](https://ping7.io) SaaS for managed Exporters for [Prometheus](https://prometheus.io/).

## Running this example project

1. Have [Docker](https://www.docker.com/products/docker-desktop) installed 🐳
1. Clone this project or download and unzip the sources 📦
1. Register with [ping7.io](https://ping7.io/signup) and activate your API key 🔥
1. Create a file named `ping7io-credentials` containing your api key 🔐

```shell
$ echo "YOUR_API_KEY" > ping7io-credentials
```

5. Use `docker compose` to launch a local Prometheus instance 🤖

```shell
$ docker compose up
```

Now you can:

* view the [configured Prometheus targets](http://localhost:9090/targets)
* query the [gathered metrics](http://localhost:9090/graph?g0.expr=probe_success&g0.tab=1&g0.stacked=0&g0.show_exemplars=0&g0.range_input=1h)
* analyze the [alarming rules](http://localhost:9090/alerts)

## Available Exporters

Under the hood we are utilizing

### Blackbox Exporter

* https://github.com/prometheus/blackbox_exporter

### SSL Exporter

* https://github.com/ribbybibby/ssl_exporter

## License

This project is licensed under the [MIT License](LICENSE).
