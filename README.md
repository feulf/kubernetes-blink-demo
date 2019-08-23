# Kubernetes Demo

Check the full demo here:
https://cloud.google.com/kubernetes-engine/docs/tutorials/external-metrics-autoscaling


**Build docker image**
```bash
docker build -t  gcr.io/google-samples/pubsub-sample:v1 .
docker push gcr.io/google-samples/pubsub-sample:v1
```

## Kubernetes

Deploy kubernetes service and deployment: 
```bash
kubectl apply -f deployments
```



