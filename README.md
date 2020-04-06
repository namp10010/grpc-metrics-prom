# grpc-metrics-prometheus
GRPC metrics demo with prometheus exporter. This is a modified version from [opencensus quickstarts](https://opencensus.io/quickstart/go/metrics/)
### Run locally

1. Clone the repo `git clone`
1. Pull prometheus docker image `docker pull prom/prometheus`
1. Run prometheus `docker run -d -v $PWD/promconfig.yml:/etc/prometheus/prometheus.yml -p 9090:9090 prom/prometheus`
1. Run main program `go run main.go`
1. See metrics at http://localhost:8888/metrics
1. Go to prometheus http://localhost:9090

### Reference

* https://opencensus.io/quickstart/go/metrics/