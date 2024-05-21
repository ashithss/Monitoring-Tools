# Kubernetes Cluster Monitoring

This repository contains configuration files for monitoring application and infrastructure logs of a Kubernetes cluster.

## Directory Structure

- `Cloudwatch/`: Contains configuration for AWS CloudWatch.
- `EFK/`: Contains configuration for Elasticsearch, Fluentd, and Kibana (EFK) stack.
- `Grafana-loki-promtail-prometheus/`: Contains configuration for Grafana, Loki, Promtail, and Prometheus.

## Cloudwatch

The `eks_cloudwatch.yaml` file in the `Cloudwatch/` directory is used to configure AWS CloudWatch for monitoring. It includes the configuration for Fluent Bit DaemonSet and the necessary parsers.

## EFK

The `EFK/` directory contains configuration files for setting up Elasticsearch, Fluentd, and Kibana. Fluentd is used to collect logs and send them to Elasticsearch. Kibana is used for visualizing the logs.

- `es_service.yaml` and `es-statefulset.yaml`: Configuration for Elasticsearch service and stateful set.
- `fluentd-es-configmap.yaml`: Configuration for Fluentd, including input and output plugins, and Prometheus exporter plugin for monitoring.
- `fluentd-es-ds.yaml`: Configuration for Fluentd DaemonSet.
- `kibana-deployment.yaml` and `kibana-service.yaml`: Configuration for Kibana deployment and service.

## Grafana-loki-promtail-prometheus

This directory contains configuration files for setting up Grafana, Loki, Promtail, and Prometheus for log monitoring and visualization.

## Setup

Provide instructions on how to use these configuration files to set up monitoring for a Kubernetes cluster.

## Contributing

Provide instructions on how to contribute to this project.

## License

Provide information about the license.