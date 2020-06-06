python-live-crowd-traking
---
To build and install the app in local
```
bash start.sh
```
or 

```
docker build -t people-counter pyimagesearch/
docker run -p 127.0.0.1:8080:8080/tcp people-counter
```
To deploy into Kubernetes Cluster

```
docker tag people-counter {dockeraccount}/crowd-tracking:{tagname}
docker push {dockeraccount}/people-counter:{tagname}
kubectl apply -f deployment.yaml
```
