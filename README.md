# Kubernetes Overview

Kubernetes is an open-source container orchestration platform designed to automate the deployment, scaling, and management of containerized applications.

## What is a POD?

In Kubernetes, a Pod is the smallest, most basic deployable object. A Pod represents a single instance of a running process in your cluster. Pods contain one or more containers, such as Docker containers. Each Pod is designed to run a single instance of a given application, thus ensuring high availability, scalability, and efficient resource management

# kubectl Helpful Commands

1. **Run**:  Create and run a particular image.
   ```bash
   kubectl run my-pod --image=my-image
   ```

2. **Describe**: Get detailed information about a resource.
   ```bash
   kubectl describe pod my-pod
   ```

3. **Get**: List resources.
   ```bash
   kubectl get pods
   ```

4. **Logs**: Print the logs from a container.
   ```bash
   kubectl logs my-pod --container=my-container
   ```

5. **Delete**: Delete resources.
   ```bash
   kubectl delete pod my-pod
   ```

6. **Expose**: Expose a resource as a new Kubernetes service.
   ```bash
   kubectl expose pod my-pod --port=8080
   ```

# What is a Cluster
A Kubernetes cluster is a set of nodes that run containerized applications. It contains at least one master node that manages multiple worker nodes.

# Difference Between Cluster and POD
A Cluster is a collection of nodes, whereas a Pod is the smallest deployable unit that holds one or more containers. Pods run on nodes within the cluster.

# What is Cluster IP and How It's Tagged to POD
ClusterIP is a type of service that provides a stable IP address to access Pods internally within the cluster. It tags the Pod for internal communication.

# What is a NodePort Service and Its Usefulness
A NodePort service exposes a service on a static port on each node’s IP address. This allows external traffic to access the service without going through the load balancer, making it simpler to route external requests to specific Pods.
