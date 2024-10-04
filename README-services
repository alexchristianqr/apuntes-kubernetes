# SERVICES

**Cluster-IP POD Service**

```bash
# Pod servicio tipo CLUSTER-IP
kubectl -n default get pods -o wide
kubectl apply -f manifests/samples-kubernetes/service-clusterip.yml
kubectl delete -f manifests/samples-kubernetes/service-clusterip.yml
kubectl describe svc hello
kubectl exec -it nginx-pod -- sh

curl http://hello:3000 # Ejemplo ping
```

**Node-Port POD Service**

```bash
# Pod servicio tipo NODE-PORT
kubectl -n default get pods -o wide
kubectl apply -f manifests/samples-kubernetes/service-nodeport.yml
kubectl delete -f manifests/samples-kubernetes/service-nodeport.yml
kubectl -n ingress-nginx get svc -o wide
kubectl describe svc hello
kubectl exec -it nginx-pod -- sh

curl http://hello:3000 # Ejemplo ping
```

**Load-Balancer POD Service**

```bash
# Pod servicio tipo LOAD-BALANCER
kubectl -n default get pods -o wide
kubectl apply -f manifests/samples-kubernetes/service-loadbalancer.yml
kubectl delete -f manifests/samples-kubernetes/service-loadbalancer.yml
kubectl describe svc hello
kubectl exec -it nginx-pod -- sh

curl http://hello:3000 # Ejemplo ping
```
