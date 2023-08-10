## How to monitor any third party application in Kubernetes 
![Screenshot_20230809-142927_YouTube ReVanced~2](https://github.com/Saurabhkr952/Observability/assets/32189783/5e74db64-72dc-42c4-a8fa-9e699cdca979)

## Metric Scraping Components

To scrape metrics, you'll need to set up three essential components:

1. **Exporter Application**:
   - This component exposes a `/metrics` endpoint.

2. **Service**:
   - For connecting to the exporter.

3. **ServiceMonitor**:
   - It helps in locating and monitoring the services that need to be connected to the exporter.

By integrating these components, you can effectively scrape, retrieve, and monitor metrics data.


## Service-Monitor 
- Define a set of target for prometheus to monitor and scrape.

<img width="935" alt="107" src="https://github.com/Saurabhkr952/Observability/assets/32189783/a37d455a-f887-4fe8-a15a-2a27274967cc">


---


```yaml
# The `prometheus.yaml` available in this repository has labels:
matchLabels:
  kubernetes.io/metadata.name: default     # This targets monitoring in the default namespace.
```

![custom](https://github.com/Saurabhkr952/Observability/assets/32189783/abb484d8-964f-45ac-9991-3ece97630b69)
