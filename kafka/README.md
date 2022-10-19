### Install Kafka operator
https://strimzi.io/docs/operators/latest/quickstart.html
```
kubectl apply -n kafka -f kafka/cluster/ 
kubectl apply -n kafka-operator -f kafka/cluster-operator/
```
