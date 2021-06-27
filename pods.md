# Creating a Pod

```
kubectl run kuard --image=gcr.io/kuar-demo/kuard-amd64:1
```

# Get the status

```
kubectl get pods
```

# Delete

```
kubectl delete deployments/kuard
```

# Running Pod

```
kubectl apply -f kuard-pod.yml
```

## Describe created pod

```
kubectl describe pods kuard
```

## Delete created pod

```
kubectl delete pods/kuard
OR
kubectl delete -f kuard-pod.yaml
```
