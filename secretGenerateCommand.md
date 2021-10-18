### Command to create secret of docker registry for Kubectl
```
kubectl create secret docker-registry --dry-run=client regcred --docker-server=https://index.docker.io/v1/ --docker-username=<username> --docker-password=<password> --docker-email=<email> -o yaml > registry-credentials.yaml
```

