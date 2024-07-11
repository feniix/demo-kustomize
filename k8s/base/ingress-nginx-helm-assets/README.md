

```bash
helm template ingress-nginx ingress-nginx --repo https://kubernetes.github.io/ingress-nginx --values k8s/base/ingress-nginx-helm-assets/helm-values.yaml --version 4.11.0 --namespace ingress-nginx --create-namespace > k8s/base/ingress-nginx-helm-assets/ingress-nginx.yaml
```