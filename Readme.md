# RabbitMq Kubernetes

### Installing RabbitMQ Cluster Operator in a Kubernetes Cluster 


RabbitMq documentation recommend install <b>versions 0.46.0+</b>.

There are diferents ways to install:

## Kubectl

You can use the last version 

```
kubectl apply -f "https://github.com/rabbitmq/cluster-operator/releases/latest/download/cluster-operator.yml"
```

or you can use a specific version

```
kubectl apply -f "https://github.com/rabbitmq/cluster-operator/releases/download/v1.11.1/cluster-operator.yml"
```

## Helm Chart 

```
helm repo add bitnami https://charts.bitnami.com/bitnami

helm install rabbitMQ-release bitnami/rabbitmq-cluster-operator
```