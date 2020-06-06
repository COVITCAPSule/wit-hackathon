wit-hackathon
===
Contains 2 Modules
1. python-live-crowd-traking (Python Application)
2. java-metro-app-ui (Springboot Application)

python-live-crowd-traking
---
Building and running in local
bash start.sh --> creates and runs a docker instance of the python app

Deploying into Kubernetes Cluster
docker tag people-counter {dockeraccount}/crowd-tracking:{tagname}
docker push {dockeraccount}/people-counter:{tagname}
kubectl apply -f deployment.yaml

java-metro-app-ui
===
Building and running
mvn clean install
java -jar target/{war}.war

