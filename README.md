# KubernetesHelmProject
***
Kubernetes project creating 2 deployment and service using Helm Charts. 

## 💻 Pre-requisites

Before you use this project you need to have Docker installed in your computer,and also Minikube.

https://www.docker.com/products/docker-desktop/
https://minikube.sigs.k8s.io/docs/start/?arch=%2Fwindows%2Fx86-64%2Fstable%2F.exe+download

### Git clone
This will clone the project:
```
$ git clone https://github.com/Kar1stan/KubernetesHelmProject.git
$ cd KubernetesHelmProject
```

## 🚀 Run the manifest: 
To deploy helm chart ,open the terminal and run:
```
$ helm install app Chart-Kar/
```
You can change deploying image and number of replicas,open the terminal and run:
```
$ helm install app1 Chart-Kar/ --set container.image=tomcat:latest --set replicaCount=3
```
If you want upgrade existing chart,open the terminal and run:
```
$  helm upgrade app Chart-Kar/ --set container.image=selenium/node-docker:latest --set replicaCount=4
```
To show list of deploys,open the terminal and run:
```
$ helm list
```
