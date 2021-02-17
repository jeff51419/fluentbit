To add the fluent helm repo, run:

```
helm repo add fluent https://fluent.github.io/helm-charts
```
To install a release named fluent-bit, run:

```
helm install --values=fluentbit-value.yaml -n far fluent-bit fluent/fluent-bit --dry-run
```

```
helm upgrade --values=fluentbit-value.yaml -n far fluent-bit fluent/fluent-bit --dry-run
```

---

To add the fluent helm repo, run:
```
helm repo add bitnami https://charts.bitnami.com/bitnami
```
To install a release named fluent-bit, run:

```
helm install --values=fluentd-value.yaml -n logging fluentd bitnami/fluentd --dry-run
```

```
helm upgrade --values=fluentd-value.yaml -n logging fluentd bitnami/fluentd --dry-run
helm upgrade -f fluentd-value.yaml -n logging fluentd bitnami/fluentd --dry-run
```


