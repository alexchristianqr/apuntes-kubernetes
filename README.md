# apuntes-kubernetes

Todo sobre kubernetes: PODS, SERVICES e INGRESS

# How use to it?

```bash
# Versión del cliente de kubernetes
kubectl version --output=yaml

# Ayuda
kubectl --help
kubectl config get-contexts

# Configuración de kubernetes en yaml
kubectl config view

# Obtener  todos los pods
kubectl get all # Ver todos los servicios de kubernetes
kubectl get namespaces # Ver nombre del espacio o grupo
kubectl get nodes # Ver nodos del orquestador kubernetes
kubectl get pods # Ver pods
kubectl get svc # Ver servicios
kubectl get pvc # Ver los volumenes
kubectl get sts # Ver statefulset
kubectl get ing # Ver ingress

# Trabajar con los manifiestos
kubectl apply -f [NAME_FILE].yml # Crear yml
kubectl delete -f [NAME_FILE].yml # Eliminar yml definitivamente de kubernetes

# Acceder a la terminal del pod a traves de la API de kubernetes
kubectl exec -it [NAME_POD] -- sh

# Obtener los eventos de un pod
kubectl describe pod [NAME_POD] # Eventos de un pod
kubectl describe svc [NAME_POD] # Eventos de un servicio

# Obtener los pods del namespace [NAME_SPACE]="kube-system"
kubectl -n [NAME_SPACE] get pods # VEr pods
kubectl -n [NAME_SPACE] get pods -o wide # Mostrar mas columnas como "IP"
kubectl -n [NAME_SPACE] get pods [NAME_POD] -o yaml # Ver yml de un pod
kubectl -n [NAME_SPACE] delete pod [NAME_POD] # Eliminar pod y kuberneter lo creará nuevamente
```

## PODS

[Todo sobre Pods](README-pods.md)


## SERVICES

[Todo sobre Services](README-services.md)


## INGRESS

[Todo sobre Ingress](README-ingress.md)
