# cortex-kustomize-demo
This is an example of monitoring Cortex by adding prometheus and grafana using kustomize


### Generate customized YAML with:

`kustomize build deploy/overlays/dev > deploy/overlays/dev/deploy.yaml`


### The YAML can be directly applied to a cluster:

`kustomize build deploy/overlays/dev | kubectl apply -f -`

or

`kustomize build https://github.com/qclaogui/cortex-kustomize-demo/deploy/overlays/dev?ref=main | kubectl apply -f -`