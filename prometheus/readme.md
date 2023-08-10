

## Service-Monitor 
- Define a set of target for prometheus to monitor and scrape.

<img width="935" alt="107" src="https://github.com/Saurabhkr952/Observability/assets/32189783/a37d455a-f887-4fe8-a15a-2a27274967cc">


---

- The `prometheus.yaml` available in this repository has labels:

```yaml
matchLabels:
  kubernetes.io/metadata.name: default          # This targets monitoring in the default namespace.
```

![custom](https://github.com/Saurabhkr952/Observability/assets/32189783/abb484d8-964f-45ac-9991-3ece97630b69)
