# DrMarkdown-infrustructure

This repo contains descriptor (yaml) files of Kubernetes objects

Some bried descriptions of How To is given below.

## About Minikube
- A tool to run kubernetes locally
- Minikube runs single node kubernetes cluster [contains master node & worker node together in the same cluster]
- Alternates are - kind, kubeadm

### Minikube commands

#### Start Minikube with docker driver
```
$ minikube start --driver=docker
```
#### Delete Minikube
```
$ minikube delete
```

## About Kubectl

- The CLI tool to interact with the kubernetes cluster.
-


### Command to create secret of docker registry for Kubectl
```
kubectl create secret docker-registry --dry-run=client regcred --docker-server=https://index.docker.io/v1/ --docker-username=<username> --docker-password=<password> --docker-email=<email> -o yaml > registry-credentials.yaml
```

