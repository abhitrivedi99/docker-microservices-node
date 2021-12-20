# Blog Application with Docker & Microservice

Microservice with Node. Using Event bus, Docker, Kubernetes.

In this Project I have built Simple React Blog app with Post and Comments functionality. Mainly focusing on Docker and Kubernetes.

### Note: I am using Ubuntu 20.04, Docker v20.10.12, Minikube v1.24.0, Kubernetes v1.22.3, Skaffold, Ingress-nginx and Node v16.13.1.

Here's the dependency installation information:
1. https://nodejs.org/en/download/
2. https://docs.docker.com/engine/install/
3. https://minikube.sigs.k8s.io/docs/start/
4. https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/
5. https://kubernetes.github.io/ingress-nginx/deploy/
6. https://skaffold.dev/docs/install/#standalone-binary

After installing dependencies run the following command:
```
- minikube start
- minikube addons enable ingress
- skaffold dev
```

Here you have to change in your hosts file to run everything on your local environment 

```
$ nano /etc/hosts
```

PASTE following in your bash config file

```
# React blog microservice based app

192.168.49.2 posts.com
```

Open react app on http://posts.com/


Enjoy!!

To stop this project and clean up your cluster, run the following command:

```
- skaffold delete
- minikube stop
```
