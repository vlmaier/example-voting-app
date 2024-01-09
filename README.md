# Example Voting App

A simple distributed application running across multiple Docker containers in k8s cluster.

This is based on the original [example-voting-app-kubernetes](https://github.com/kodekloudhub/example-voting-app-kubernetes?tab=readme-ov-file).

## Run

```shell
kubectl create -f voting-app-deploy.yml
kubectl create -f result-app-deploy.yml
kubectl create -f worker-app-deploy.yml
kubectl create -f redis-deploy.yml
kubectl create -f postgres-deploy.yml
kubectl create -f voting-app-service.yml
kubectl create -f result-app-service.yml
kubectl create -f redis-service.yml
kubectl create -f postgres-service.yml
```