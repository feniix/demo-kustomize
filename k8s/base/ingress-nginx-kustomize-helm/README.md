# Build and deploy to kubernetes

```bash
kustomize build --enable-helm k8s/base/ingress-nginx-kustomize-helm | kubectl apply --server-side --force-conflicts -f-
```
