# Generate assets

```bash
curl -sL https://github.com/kubernetes/ingress-nginx/blob/controller-v1.11.0/deploy/static/provider/cloud/deploy.yaml > k8s/base/ingress-nginx-curl-assets/ingress-nginx.yaml
```

# Build and push deploy

```bash
kustomize build k8s/base/ingress-nginx-curl-assets/ | kubectl apply --server-side --force-conflicts -f-
```
