### Install ArgoCD
```
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
```

### Port-forward
```
kubectl port-forward service/argo-cd-argocd-server -n argocd 8080:443
```
