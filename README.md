# infra-k8s-default-apps

## Prerequisites
- Install kubectl
- Have a Kubernetes Cluster and add its kubeconfig

## Get started
Install ArgoCD on your Kubernetes Cluster:
```
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
```
Log in to ArgoCD and add this repo to your ArgoCD:
```
https://github.com/stearz/infra-k8s-default-apps.git
```
Add the /core path of the above repository as an app in ArgoCD.