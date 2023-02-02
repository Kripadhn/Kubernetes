Deploy a pod:
kubectl run mypod --image=nginx --replicas=2 --port=80

Create a deployment:
kubectl create deployment mydeployment --image=nginx

Scale a deployment:
kubectl scale deployment mydeployment --replicas=3

Expose a deployment as a service:
kubectl expose deployment mydeployment --port=80 --type=ClusterIP

Get the status of a deployment:
kubectl get deployment mydeployment

Get the status of pods:
kubectl get pods

Get the status of services:
kubectl get services

Get logs for a pod:
kubectl logs mypod

SSH into a running pod:
kubectl exec -it mypod -- /bin/bash

Delete a deployment:
kubectl delete deployment mydeployment

Update a deployment:
kubectl set image deployment mydeployment mycontainer=newimage

Get details about a resource:
kubectl describe deployment mydeployment

List all pods in a namespace:
kubectl get pods --namespace=mynamespace

List all services in a namespace:
kubectl get services --namespace=mynamespace

Create a namespace:
kubectl create namespace mynamespace

Apply a configuration file:
kubectl apply -f myconfig.yml

Port forward from a local machine to a pod:
kubectl port-forward mypod 8080:80

Get events in a namespace:
kubectl get events --namespace=mynamespace

Get the version of the Kubernetes cluster:
kubectl version

Get the IP addresses of nodes in a cluster:
kubectl get nodes -o wide


Label a node:
kubectl label node mynode label=value

Get all nodes labeled with a specific label:
kubectl get nodes -l label=value

Get all resources of a specific type in a namespace:
kubectl get all --namespace=mynamespace

Get resource usage statistics for a node:
kubectl describe node mynode | grep -i resource

Edit a resource in-place:
kubectl edit deployment mydeployment

Create a secret:
kubectl create secret generic mysecret --from-literal=key=value

Get the value of a secret:
kubectl get secret mysecret -o yaml

Create a configMap:
kubectl create configmap myconfigmap --from-literal=key=value

Get the value of a configMap:
kubectl get configmap myconfigmap -o yaml

Create a persistent volume:
kubectl apply -f mypv.yaml


Scale a deployment:
kubectl scale deployment mydeployment --replicas=3

Expose a deployment as a service:
kubectl expose deployment mydeployment --type=NodePort

Get the logs of a pod:
kubectl logs mypod

Open a shell to a running container:
kubectl exec -it mypod -- /bin/bash

Delete a resource:
kubectl delete deployment mydeployment

Delete all resources in a namespace:
kubectl delete all --namespace=mynamespace

Rollback a deployment to a previous version:
kubectl rollout undo deployment mydeployment

Get the public IP address of a service:
kubectl get service myservice -o jsonpath="{.status.loadBalancer.ingress[0].ip}"

Get the public URL of a service:
kubectl get service myservice -o jsonpath="{.status.loadBalancer.ingress[0].hostname}"

Save the state of a cluster to a file:
kubectl cluster-info dump > mycluster.txt