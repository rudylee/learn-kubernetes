# Check the version

```
kubectl version
```

# Check the cluster health

```
kubectl get componentstatuses
```

# Get the list of nodes

```
kubectl get nodes
```

# More information about a node

```
kubectl describe nodes node-1
```

# Proxy

Proxy is responsible for routing network traffic to load-balanced services in the cluster.

```
kubectl get daemonSets --namespace=kube-system kube-proxy
```

# DNS

Kubernetes runs this to provide naming and discovery for services in the cluster.

```
kubectl get deployments --namespace=kube-system coredns
```

```
kubectl get services --namespace=kube-system kube-dns
```

# GUI

```
kubectl get deployments --namespace=kube-system kubernetes-dashboard
```

```
kubectl get services --namespace=kube-system kubernetes-dashboard
```

Access the UI

```
kubectl proxy
```

And the visit the UI on `http://ip:8001`

# Namespace

# Contexts

Create a new context

```
kubectl config set-context my-context --namespace=mystuff
```

Use a context

```
kubectl config use-context my-context
```

# Kubectl Get

```
kubectl get pods my-pod -o jsonpath --template={.status.podIP}<Paste>
```

```
kubectl describe <resource-name> <obj-name>
```
