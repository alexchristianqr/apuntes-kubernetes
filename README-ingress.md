# INGRESS

```bash
kubectl -n default get pods -o wide

kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.0.0/deploy/static/provider/cloud/deploy.yaml
kubectl delete -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.0.0/deploy/static/provider/cloud/deploy.yaml
kubectl get pods --all-namespaces -l app.kubernetes.io/name=ingress-nginx
kubectl get services ingress-nginx-controller --namespace=ingress-nginx

kubectl -n ingress-nginx get svc
kubectl apply -f manifests/samples-kubernetes/ingress-nginx.yml
kubectl delete -f manifests/samples-kubernetes/ingress-nginx.yml
kubectl get ing

curl http://kubernetes.docker.internal/v2 # Ejemplo de switch
```
