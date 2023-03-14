# Reddit Clone App via K8S using AWS EKS
This project demonstrates how to deploy a Reddit clone app on Kubernetes with Ingress and expose it to the world using Minikube as the cluster.

# Project Summary:

1. The Reddit clone application is deployed via K8S cluster on AWS EKS integrated with Ansible, Docker, Jenkins, Docker Hub & GitHub.
2. When any change happens on app code, the CI job is automatically triggered and Ansible Playbook executes, that build Docker image & push it to Docker Hub. Then CD job is triggered and Ansible Playbook runs Pods on EKS cluster from Deployment & Service manifest file.
3. After that we can access Reddit app by using Load Balancer's DNS with target port.
