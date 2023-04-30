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

### Resource Management
13. ```kubectl create -f <yaml-file>```: Create a Kubernetes resource from a YAML file.
14. ```kubectl apply -f <yaml-file>```: Apply changes to a Kubernetes resource from a YAML file.
15. ```kubectl delete <resource-type> <resource-name>```: Delete a Kubernetes resource by name and type.
16. ```kubectl edit <resource-type> <resource-name>```: Edit a Kubernetes resource by name and type.
17. ```kubectl get events```: List all events in the cluster.

### ReplicaSet Management
18. ```kubectl get replicasets```: List all replica sets in the default namespace.
19. ```kubectl describe replicasets <replicaset-name>```: Display detailed information about a specific replica set.
20. ```kubectl create replicaset <replicaset-name> --image=<image-name>```: Create a new replica set.
21. ```kubectl delete replicaset <replicaset-name>```: Delete a replica set.

### Deployment Management
22. ```kubectl get deployments```: List all deployments in the default namespace.
23. ```kubectl describe deployment <deployment-name>```: Display detailed information about a specific deployment.
24. ```kubectl rollout status deployment/<deployment-name>```: Show the status of a deployment rollout.
25. ```kubectl rollout history deployment/<deployment-name>```: Show the rollout history of a deployment.
26. ```kubectl rollout undo deployment/<deployment-name>```: Undo the last deployment rollout.
27. ```kubectl scale deployment <deployment-name> --replicas=<number-of-replicas>```: Scale a deployment by name.

### Namespace Management
28. ```kubectl get namespaces```: List all namespaces in the cluster.
29. ```kubectl create namespace <namespace-name>```: Create a new namespace.
30. ```kubectl delete namespace <namespace-name>```: Delete a namespace and all its resources.
31. ```kubectl config set-context --current --namespace=<namespace-name>```: Set the default namespace for the current context.
32. ```kubectl get all -n <namespace-name>```: List all resources in a namespace.

### Service Management
33. ```kubectl get services```: List all services in the default namespace.
34. ```kubectl describe service <service-name>```: Display detailed information about a specific service.
35. ```kubectl delete service <service-name>```: Delete a service by name.

### DaemonSet management

36. ```kubectl get daemonsets```: List all DaemonSets in the default namespace.
37. ```kubectl describe daemonset <daemonset-name>```: Display detailed information about a specific DaemonSet.
38. ```kubectl create daemonset <daemonset-name> --image=<image-name>```: Create a new DaemonSet.
39. ```kubectl delete daemonset <daemonset-name>```: Delete a DaemonSet.

### StatefulSet Management
40. ```kubectl get statefulsets```: List all stateful sets in the default namespace.
41. ```kubectl describe statefulset <stateful-set-name>```: Display detailed information about a specific stateful set.
42. ```kubectl create statefulset <stateful-set-name> --image=<image-name>```: Create a new stateful set.
43. ```kubectl delete statefulset <stateful-set-name>```: Delete a specific stateful set


### Configuration Management
44. ```kubectl config view```: View the current Kubernetes configuration.
45. ```kubectl config use-context <context-name>```: Switch to a different context.
46. ```kubectl config set-context <context-name> --cluster=<cluster-name> --user=<user-name> --namespace=<namespace-name>```: Create a new context.
47. ```kubectl config delete-context <context-name>```: Delete a context.

### Secret Management
48. ```kubectl get secrets```: List all secrets in the default namespace.
49. ```kubectl create secret generic <secret-name> --from-literal=<key>=<value>```: Create a secret from a literal value.
50. ```kubectl create secret generic <secret-name> --from-file=<path-to-file>```: Create a secret from a file.
51. ```kubectl describe secret```: Show details of a specific secret.
52. ```kubectl delete secret```: Delete a secret.

### PV (Persistent Volume) & PVC (Persistent Volume Claim) 

53. ```kubectl get pv```: View all the Persistent Volumes in the cluster.
54. ```kubectl describe pv <pv-name>```: Describe a specific Persistent Volume.
55. ```kubectl delete pv <pv-name>```: Delete a specific Persistent Volume.
56. ```kubectl get pvc```: View all the Persistent Volume Claims in the cluster.
57. ```kubectl describe pvc <pvc-name>```: Describe a specific Persistent Volume Claim.
58. ```kubectl delete pvc <pvc-name>```: Delete a specific Persistent Volume Claim.
59. ```kubectl apply -f <pv-definition-file.yaml>```: Create a Persistent Volume from a definition file.
60. ```kubectl edit pv <pv-name>```: Edit a specific Persistent Volume.
61. ```kubectl apply -f <pvc-definition-file.yaml>```: Create a Persistent Volume Claim from a definition file.
62. ```kubectl edit pvc <pvc-name>```: Edit a specific Persistent Volume Claim.
63. ```kubectl get storageclass```: View all the available storage classes in the cluster.
64. ```kubectl describe storageclass <storage-class-name>```: Describe a specific storage class.

### Ingress Management
65. ```kubectl get ingress```: List all ingresses in the default namespace.
66. ```kubectl describe ingress <ingress-name>```: Display detailed information about a specific ingress.
67. ```kubectl create ingress <ingress-name> --rule=<host>=<path>:<service>:<port>```: Create a new ingress rule.
68. ```kubectl delete ingress <ingress-name>```: Delete a specific ingress.



