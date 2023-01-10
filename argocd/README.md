### Install ArgoCD
```
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
```

### Access ArgoCD
#### 1. Port-forward
```
kubectl port-forward service/argo-cd-argocd-server -n argocd 8080:443
```
#### 2. Go to
```
https://localhost:8080/
```
#### 3. Credentials
##### Login: 
```
Admin
```
##### Password: 
```
kubectl get secret -n argocd argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 --decode
```
