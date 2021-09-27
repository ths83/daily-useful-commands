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
k config set-context --current --namespace default
