# PODS

**Single POD**

```bash
# Pod tipo POD
kubectl -n default get pods
kubectl apply -f manifests/samples-kubernetes/pod.yml
kubectl delete -f manifests/samples-kubernetes/pod.yml
kubectl -n default get pods nginx-pod -o yaml
kubectl -n default delete pod nginx-pod
```

**Deployment POD**

```bash
# Pod tipo DEPLOYMENT
kubectl -n default get pods -o wide
kubectl apply -f manifests/samples-kubernetes/pod-deployment.yml
kubectl delete -f manifests/samples-kubernetes/pod-deployment.yml
kubectl -n default get pods nginx-deployment-ID -o yaml
kubectl -n default delete pod nginx-deployment-ID
```

**Daemon-Set POD**

```bash
# Pod tipo DAEMON-SET
kubectl -n default get pods -o wide
kubectl apply -f manifests/samples-kubernetes/pod-daemonset.yml
kubectl delete -f manifests/samples-kubernetes/pod-daemonset.yml
kubectl -n default get pods nginx-daemonset-ID -o yaml
kubectl -n default delete pod nginx-daemonset-ID
```
