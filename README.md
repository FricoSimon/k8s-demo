
## Deployment

To deploy this project run these commands:

Start minikube and docker
```bash
  minikube start 
```
Create mongo config first
```bash
  kubectl apply -f mongo-config.yaml
```
Create mongo secret
```bash
  kubectl apply -f mongo-secret.yaml
```
Deploy mongo db 
```bash
  kubectl apply -f mongo.yaml
```
Deploy webapp
```bash
  kubectl apply -f webapp.yaml
```
Check the service from external 
```bash
  minikube service webapp-service
```

## Tech Stack

**Prerequisites:** Docker 

**Server:** Minikube, Kubernetes

**Tools:** Visual Studio Code, Browser (Chrome)

## Reference

Thanks to TechWorld with Nana (Youtube)

[Kubernetes Crash Course for Absolute Beginners](https://www.youtube.com/watch?v=s_o8dwzRlu4&ab_channel=TechWorldwithNana)
