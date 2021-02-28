### Kubernetes Instructions  
  
1. Create a Dockerfile: see auth Dockerfile and .dockerignore

```
docker login
sudo docker build -t havyx/auth .
```
  
* Kubernetes commands: (After minikube installation + minikube start)
```
kubectl apply -f auth-depl.yaml
kubectl get deployments
kubectl get services
kubectl delete -f auth-depl.yaml
```
  
* Adding Skaffold:  https://skaffold.dev/docs/install/
```
skaffold dev
```
