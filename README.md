# ☸️ Kubernetes (K8s) Learning Notes

A centralized repository for Kubernetes concepts, commands, and manifests.

## 📂 Quick Links
*   📖 **[Core Concepts](./01-concepts/basics.md)**: Pods, Nodes, and Clusters.
*   🌐 **[Networking](./01-concepts/networking.md)**: ClusterIP, NodePort, and Services.
*   🏗️ **[Manifests](./05-manifests/)**: Example YAML files.

---

## 📜 Why Kubernetes? The Problem It Solves

Kubernetes was created to address the growing challenges of container orchestration, scaling, and deployment complexity in modern software development. As organizations increasingly adopted containerization to improve development agility, they faced several significant issues:

1. **Container Orchestration Challenges**: Managing a large number of containers across multiple hosts can be complex. Kubernetes automates the deployment, scaling, and management of containerized applications, making it easier for developers to orchestrate their containers effectively.

2. **Scaling Issues**: As applications grow, the need to scale up or down becomes crucial. Kubernetes provides powerful scaling capabilities, allowing applications to automatically adjust the number of active instances based on current demand, ensuring optimal performance without manual intervention.

3. **Deployment Complexity**: With applications consisting of multiple microservices, coordinating deployment becomes increasingly complicated. Kubernetes enables seamless rollouts and rollbacks, providing a more straightforward approach to deploying updates while minimizing downtime and ensuring application availability.

By addressing these challenges, Kubernetes helps streamline the development and deployment processes, allowing organizations to focus on building efficient, resilient applications in a cloud-native environment.

---

## 🚀 Essential kubectl Commands
*The most common commands for managing resources.*


| Action | Command |
| :--- | :--- |
| **Run Pod** | `kubectl run my-pod --image=nginx` |
| **List Resources** | `kubectl get pods,svc,nodes` |
| **Deep Dive** | `kubectl describe pod <name>` |
| **Check Logs** | `kubectl logs -f <name>` |
| **Expose App** | `kubectl expose pod <name> --port=8080` |
| **Cleanup** | `kubectl delete pod <name>` |

---

## 🧠 At a Glance: Architecture
Kubernetes automates the deployment and scaling of containers.
- **Cluster**: The entire set of nodes (Master + Workers).
- **Node**: A physical or virtual machine in the cluster.
- **Pod**: The smallest unit (one or more containers).