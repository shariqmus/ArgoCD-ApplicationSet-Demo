# ArgoCD ApplicationSet Demo



## Installation

```

kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
```

## Connect to ArgoCD
```
kubectl port-forward svc/argocd-server -n argocd 8080:443
brew install argocd
argocd admin initial-password -n argocd

BKS***************
```

## Browse to:

https://localhost:8080/



## Add clusters
```
argocd login localhost:8080
argocd version
argocd cluster add do-lon1-engineering-dev
argocd cluster add do-lon1-engineering-prod
```
