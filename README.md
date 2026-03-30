# ☸️ Kubernetes (K8s) Learning Notes

A centralized repository for Kubernetes concepts, commands, and manifests.

## 📂 Quick Links
*   📖 **[Core Concepts](./01-concepts/basics.md)**: Pods, Nodes, and Clusters.
*   🌐 **[Networking](./01-concepts/networking.md)**: ClusterIP, NodePort, and Services.
*   🏗️ **[Manifests](./05-manifests/)**: Example YAML files.

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
