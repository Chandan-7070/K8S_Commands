1. General Information Commands

Command	                        Description
kubectl version              	Show the Kubernetes version.
kubectl cluster-info    	    Display cluster info.
kubectl get all	                Get all resources in the namespace.
kubectl config view	            Display kubeconfig settings.
kubectl api-resources     	    List all API resources.
kubectl api-versions	        List all API versions.


2. Namespace Management
Command	                         Description
kubectl get namespaces	           List all namespaces.
kubectl create namespace <name>	   Create a namespace.
kubectl delete namespace <name>	   Delete a namespace.
kubectl config set-context --current --namespace=<name>	    Set current namespace.



3. Pod Management
Command	                         Description
kubectl get pods	             List all pods.
kubectl get pods -o wide	     List pods with detailed info.
kubectl describe pod <name>	     Describe a specific pod.
kubectl delete pod <name>	     Delete a pod.
kubectl logs <pod-name>	         View pod logs.
kubectl exec -it <pod-name> -- <command>	Execute a command in a pod.


4. Deployment Management
Command	                                            Description
kubectl get deployments	                            List deployments.
kubectl describe deployment <name>	                Describe a deployment.
kubectl create deployment <name> --image=<image>	Create a deployment.
kubectl scale deployment <name> --replicas=<n>	     Scale deployment replicas.
kubectl rollout restart deployment/<name>	         Restart a deployment.
kubectl delete deployment <name>	                 Delete a deployment.

5. Service Management
Command	                                                    Description
kubectl get services	                                    List services.
kubectl describe service <name>        	                    Describe a service.
kubectl expose pod <pod-name> --type=<type> --port=<port>	Expose a pod as a service.
kubectl delete service <name>	                             Delete a service.


6. ConfigMap and Secret Management
Command                                                                 	Description
kubectl get configmaps	                                                   List ConfigMaps.
kubectl describe configmap <name>	                                       Describe a ConfigMap.
kubectl create configmap <name> --from-literal=<key>=<value>	           Create a ConfigMap.
kubectl delete configmap <name>                          	               Delete a ConfigMap.
kubectl get secrets	                                                        List secrets.
kubectl create secret generic <name> --from-literal=<key>=<value>	       Create a secret.
kubectl describe secret <name>	                                           Describe a secret.


7. Node Management
Command	                                        Description
kubectl get nodes	                            List nodes.
kubectl describe node <name>	                Describe a node.
kubectl cordon <node-name>	                    Mark a node as unschedulable.
kubectl drain <node-name>	                    Safely evict pods from a node.
kubectl uncordon <node-name>	                Mark a node as schedulable.


Here is a comprehensive list of commonly used Kubernetes commands, grouped by purpose. These commands are executed using the kubectl CLI tool.

1. General Information Commands
Command	Description
kubectl version	Show the Kubernetes version.
kubectl cluster-info	Display cluster info.
kubectl get all	Get all resources in the namespace.
kubectl config view	Display kubeconfig settings.
kubectl api-resources	List all API resources.
kubectl api-versions	List all API versions.
2. Namespace Management
Command	Description
kubectl get namespaces	List all namespaces.
kubectl create namespace <name>	Create a namespace.
kubectl delete namespace <name>	Delete a namespace.
kubectl config set-context --current --namespace=<name>	Set current namespace.
3. Pod Management
Command	Description
kubectl get pods	List all pods.
kubectl get pods -o wide	List pods with detailed info.
kubectl describe pod <name>	Describe a specific pod.
kubectl delete pod <name>	Delete a pod.
kubectl logs <pod-name>	View pod logs.
kubectl exec -it <pod-name> -- <command>	Execute a command in a pod.
4. Deployment Management
Command	Description
kubectl get deployments	List deployments.
kubectl describe deployment <name>	Describe a deployment.
kubectl create deployment <name> --image=<image>	Create a deployment.
kubectl scale deployment <name> --replicas=<n>	Scale deployment replicas.
kubectl rollout restart deployment/<name>	Restart a deployment.
kubectl delete deployment <name>	Delete a deployment.
5. Service Management
Command	Description
kubectl get services	List services.
kubectl describe service <name>	Describe a service.
kubectl expose pod <pod-name> --type=<type> --port=<port>	Expose a pod as a service.
kubectl delete service <name>	Delete a service.
6. ConfigMap and Secret Management
Command	Description
kubectl get configmaps	List ConfigMaps.
kubectl describe configmap <name>	Describe a ConfigMap.
kubectl create configmap <name> --from-literal=<key>=<value>	Create a ConfigMap.
kubectl delete configmap <name>	Delete a ConfigMap.
kubectl get secrets	List secrets.
kubectl create secret generic <name> --from-literal=<key>=<value>	Create a secret.
kubectl describe secret <name>	Describe a secret.
7. Node Management
Command	Description
kubectl get nodes	List nodes.
kubectl describe node <name>	Describe a node.
kubectl cordon <node-name>	Mark a node as unschedulable.
kubectl drain <node-name>	Safely evict pods from a node.
kubectl uncordon <node-name>	Mark a node as schedulable.


8. Resource Editing
Command	                                                     Description
kubectl edit <resource> <name>	                              Edit a resource in-place.
kubectl patch <resource> <name> --patch=<json/yaml>     	Apply a patch to a resource. 

9. Troubleshooting Commands
Command	                                        Description
kubectl get events	                            View cluster events.
kubectl logs <pod-name>	                         Check logs for a pod.
kubectl describe <resource> <name>	               Detailed info about a resource.
kubectl debug <pod-name>	                        Debug a running pod. 


10. YAML File Commands
Command	                                 Description
kubectl apply -f <file.yaml>	   Create/update resources from a file.
kubectl delete -f <file.yaml>	  Delete resources from a file.
kubectl get -f <file.yaml>	      Display resources defined in a file.