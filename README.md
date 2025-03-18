## Self-managed helm chart repo

- cert-manager-webhook-ovh-chart
- execution-beacon

## Build the chart
```
# execution-beacon folder
helm package execution-beacon

# Repo root folder
helm repo index --url https://nm-sam.github.io/cust-helm-charts/ --merge index.yaml .
```

## Install and test
```
helm repo add myrepo https://nm-sam.github.io/cust-helm-charts/
helm repo list
helm repo update
helm search repo myrepo

helm install test-beacon myrepo/execution-beacon --version 1.0.11

```
