## Steps I took to complete the assingment:



## Commands:
cd assignment3
minikube start
minikube addons enable ingress

### To apply each file:
kubectl apply -f nginx-dep.yml
kubectl apply -f nginx-configmap.yml
kubectl apply -f nginx-svc.yml
kubectl apply -f nginx-ingress.yml
kubectl apply -f app-1-dep.yml
kubectl apply -f app-1-svc.yml
kubectl apply -f app-1-ingress.yml
kubectl apply -f app-2-dep.yml
kubectl apply -f app-2-svc.yml
kubectl apply -f app-2-ingress.yml

### To get deployments, services and ingresses
kubectl get deployments
kubectl get services
kubectl get ingresses

### To get responses from the load-balanced apps
curl http://(minikube ip)/

