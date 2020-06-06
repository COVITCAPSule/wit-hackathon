wit-hackathon
==================
Contains 2 Modules
1. python-live-crowd-traking (Python Application)
2. java-metro-app-ui (Springboot Application)

python-live-crowd-traking
---
To build and install the app in local

  bash start.sh

or 

  docker build -t people-counter pyimagesearch/
  docker run -p 127.0.0.1:8080:8080/tcp people-counter

To deploy into Kubernetes Cluster

  docker tag people-counter {dockeraccount}/crowd-tracking:{tagname}
  docker push {dockeraccount}/people-counter:{tagname}
  kubectl apply -f deployment.yaml

java-metro-app-ui
===
To build and install the app in local

  mvn clean install
  java -jar target/{war}.war

