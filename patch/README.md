## Apply Configurations

```bash
kubectl create ns cert-manager && 
kubectl create -n cert-manager secret generic cloudflare-api-token \    --from-literal=access-token=<insert access token>
```

### ArgoCD Ingress

```bash
kubectl apply -f argo-ingress.yaml
```