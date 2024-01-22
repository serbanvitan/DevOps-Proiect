This project demonstrates the deployment of a minimal Kubernetes application using Minikube. The application consists of a basic "Hello World" web server, and the deployment is orchestrated using key Kubernetes components such as Pods, Services, and Deployments.

Components:
Docker Image:

A Docker image is created for the "Hello World" web server using the lightweight Nginx server with the Alpine Linux base. Alpine Linux is chosen for its minimal size, contributing to efficient resource usage and quicker download times.

Kubernetes Deployment:

A Kubernetes Deployment is defined in the hello-world-deployment.yaml file. This deployment ensures the desired number of replicas of the "Hello World" pod are running. The pod uses the Docker image created earlier.

Kubernetes Service:

A Kubernetes Service (hello-world-service) is defined in the hello-world-service.yaml file. This service exposes the deployed pods, allowing them to be accessed within the Kubernetes cluster.

Exposing the Service:

The kubectl port-forward command is used to forward local ports to the deployed service, enabling access to the "Hello World" application within the Kubernetes cluster from the local machine.

Objective:
The primary goal of this project is to illustrate the deployment of a simple application within a local Kubernetes cluster using Minikube. By following the outlined steps, users gain practical experience with Kubernetes concepts and learn to troubleshoot common deployment issues.
