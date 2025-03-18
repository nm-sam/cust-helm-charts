# cert-manager-webhook-ovh-chart

# execution-beacon folder
helm package execution-beacon

# Repo root folder
helm repo index --url https://nm-sam.github.io/cust-helm-charts/ --merge index.yaml .
