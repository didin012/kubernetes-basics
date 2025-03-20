# Kubernetes Basics ![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)
This is a repo that contains some basic ````kubectl```` commands.
## Creating resource from a YAML file
Suppose that you have ````deployment-definition.yml```` file in your current directory <br>
````
$ kubectl create -f deployment-definition.yml
````
## Deleting a resource
````
$ kubectl delete -f deployment-definition.yml
````
## Some K8s Components
We have different components in kubernetes that you may encounter
### Minikube
````minikube```` is a tool that lets you run Kubernetes locally. minikube runs an all-in-one or a multi-node local Kubernetes cluster on your personal computer (including Windows, macOS and Linux PCs) so that you can try out Kubernetes, or for daily development work.
### Cluster

### Node
Kubernetes runs your workload by placing containers into Pods to run on Nodes. A node may be a virtual or physical machine, depending on the cluster.
### Pods
Pods are the smallest deployable units of computing that you can create and manage in Kubernetes.
### Service
Service is a method for exposing a network application that is running as one or more Pods in your cluster.
### Deployment

## Checking Pods
````
$ kubectl get pods
````
## Checking ReplicaSet
````
$ kubectl get replicaset
````
## Checking Deployments
````
$ kubectl get deployment
````
## Checking Services
````
$ kubectl get svc
````
## Checking Namespaces
````
$ kubectl get ns
````
## Checking Pods Inside a Namespace
````
$ kubectl get -n <namespace>
````
## Editing a Deployment
````
$
````

 1. Get nodes: `kubectl get nodes`
 2. Get pods: `kubectl get pods`
 3. Get deployments: `kubectl get deployments`
 4. Get services: `kubectl get svc`
 5. Create a deployment: `kubectl create deployment <deployment_name> --image=<image_name>`
 6. Apply a configuration: `kubectl apply -f <config_file>`
 7. Get pod logs: `kubectl logs <pod_name>`
 8. Exec into a pod: `kubectl exec -it <pod_name> -- /bin/bash`
 9. Scale a deployment: `kubectl scale deployment <deployment_name> --replicas=<replica_count>`
 10.Delete a po: `kubectl delete pod <pod_name>`

