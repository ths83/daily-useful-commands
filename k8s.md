https://github.com/wercker/stern
brew install stern

https://eksctl.io/
brew install eksctl

https://github.com/ahmetb/kubectx
brew install kubectx

---
### Create alias command
alias k=kubectl

### Get live access to pod's bash container
k exec <POD_NAME> -c <POD_CONTAINER_NAME> -it -- /bin/sh

### Set kubectl current namespace
k config set-context --current --namespace <NS>
  
### List alive resources in the given namespace
kubectl api-resources --verbs=list --namespaced -o name | xargs -n 1 kubectl get --show-kind --ignore-not-found -n <NS>
  
### Force resource deletion in the given namespace (ONLY when deletion in too long)
kubectl -n <NS> patch <K8S_RESOURCE> <RESOURCE_NAME> -p '{"metadata":{"finalizers":[]}}' --type=merge
