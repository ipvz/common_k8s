## Install
### Add helm repo
```
helm repo add bitnami https://charts.bitnami.com/bitnami
```
### Helm install
```
helm install mongo -n mongo bitnami/mongodb
```
### Root credentials
```
kubectl get secret --namespace mongo mongo-mongodb -o jsonpath="{.data.mongodb-root-password}" | base64 -d
```
