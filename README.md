# Promtail for JSON logging
Helm chart of Loki stack with Promtail configured to parse JSON logs.

## TL;DR

```console
helm dependency update
helm install promtail-json-parser /promtail-json-parser -f /promtail-json-parser/values.yaml
```

## Notes

Promtail pipeline stage depends on Container Runtaim used by Kubernetes node

- [CRI stage](https://grafana.com/docs/loki/latest/clients/promtail/stages/cri/) should be used for containerd runtime
- [Docker stage](https://grafana.com/docs/loki/latest/clients/promtail/stages/docker/) should be used for Docker Engine runtime 