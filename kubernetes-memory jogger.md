### Cluster Management

1. ```kubectl version```: Show the version of kubectl and the Kubernetes server.
2. ```kubectl cluster-info```: Display information about the Kubernetes cluster.
3. ```kubectl get nodes```: List all nodes in the cluster.
4. ```kubectl describe node <node-name>```: Display detailed information about a specific node.
5. ```kubectl top node```: Show CPU and memory usage for all nodes.

### Pod Management
6. ```kubectl get pods```: List all pods in the default namespace.
7. ```kubectl describe pod <pod-name>```: Display detailed information about a specific pod.
8. ```kubectl logs <pod-name>```: Display logs for a specific pod.
9. ```kubectl exec <pod-name> -- <command>```: Run a command in a specific pod.
10. ```kubectl attach <pod-name> -c <container-name>```: Attach to a running container in a pod.
11. ```kubectl delete pod <pod-name>```: Delete a pod by name.
12. ```kubectl get pod <pod-name> -o yaml```: Get the YAML configuration of a pod.

### Deployment Management
13. ```kubectl get deployments```: List all deployments in the default namespace.
14. ```kubectl describe deployment <deployment-name>```: Display detailed information about a specific deployment.
15. ```kubectl rollout status deployment/<deployment-name>```: Show the status of a deployment rollout.
16. ```kubectl rollout history deployment/<deployment-name>```: Show the rollout history of a deployment.
17. ```kubectl rollout undo deployment/<deployment-name>```: Undo the last deployment rollout.
18. ```kubectl scale deployment <deployment-name> --replicas=<number-of-replicas>```: Scale a deployment by name.

### Service Management
19. ```kubectl get services```: List all services in the default namespace.
20. ```kubectl describe service <service-name>```: Display detailed information about a specific service.
21. ```kubectl delete service <service-name>```: Delete a service by name.

### Namespace Management
22. ```kubectl get namespaces```: List all namespaces in the cluster.
23. ```kubectl create namespace <namespace-name>```: Create a new namespace.
24. ```kubectl delete namespace <namespace-name>```: Delete a namespace and all its resources.
25. ```kubectl config set-context --current --namespace=<namespace-name>```: Set the default namespace for the current context.
26. ```kubectl get all -n <namespace-name>```: List all resources in a namespace.

### Resource Management
27. ```kubectl create -f <yaml-file>```: Create a Kubernetes resource from a YAML file.
28. ```kubectl apply -f <yaml-file>```: Apply changes to a Kubernetes resource from a YAML file.
29. ```kubectl delete <resource-type> <resource-name>```: Delete a Kubernetes resource by name and type.
30. ```kubectl edit <resource-type> <resource-name>```: Edit a Kubernetes resource by name and type.
31. ```kubectl get events```: List all events in the cluster.
