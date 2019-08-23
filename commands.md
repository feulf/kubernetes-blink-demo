Send multiple message into pubsub
```
for i in {1..200}; do gcloud pubsub topics publish echo --message="Autoscaling #${i}"; done
:x
```

Read messages from pubsub
```bash
gcloud pubsub subscriptions pull --auto-ack refill-listener
```

## Cluster
Resizing the cluster
```bash
gcloud container clusters list
gcloud container clusters describe [CLUSTER_NAME] # get the node-pool name
gcloud container clusters resize [CLUSTER_NAME] --node-pool [POOL_NAME] --num-nodes [NUM_NODES]
```

## Daemon
```bash
kubectl get daemonset
```

Useful commands:
```
kubectl logs pod-name -f
kubectl exec -it my-pod --container main-app -- /bin/bash  # get a shell
kubectl create secret generic pubsub-key --from-file=PATH-TO-FILE.json  # create kube secrets
kubectl scale --replicas=10 deploy/pubsub
```
