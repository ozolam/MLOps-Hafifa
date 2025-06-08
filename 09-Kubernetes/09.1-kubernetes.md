# Kubernetes

During this section, you are meant to understand the basic concepts of Kubernetes (K8s), its role in cloud-native infrastructure, and how we use it to support machine learning workflows.

---

### TODO:

1. [Google what Kubernetes is](https://letmegooglethat.com/?q=what+is+kubernetes)
2. Read the official [Kubernetes overview](https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/)
3. Read this article [Kubernetes in ML workflows](https://towardsdatascience.com/kubernetes-for-machine-learning-deployments-c24c988d72f4)
4. Explore the Kubernetes services currently running in our team or company (you can ask your hofef for a list).
5. Identify how Kubernetes supports the lifecycle of ML workflows (training, serving, batch jobs, monitoring).

---

### Key Concepts:

- Basics:
  - What is kubernetes?
  - What is kubernetes resource?
  - what is manifest?
  - what is YAML?
  - what is kubernetes api?
  - what is the main template of all kubernetes resources?
  - what is Kubectl?  
- Cluster
  - What is the purpose of kubernetes cluster?
  - what is the structure of kubernetes cluster?  
- Pod 
  - What is the different between pod and container?
  - Why would you use multiple containers in on pod?
  - What is init container?
  - Look at a pod manifest
- ReplicaSet 
- Deployment
  - What are the differences between deployment and replicaSet?
  - Why would we prefer to deploy a deployment and not a pod?
- PersistentVolume
- PersistentVolumeClaim
  - Why do you need both PV and PVC?
- StorageClass
  - look at examples!
- StatefulSet
  - What are the main differences between StatefulSet and Deployment?     
- Service
- Ingress  
- Node  
- Namespace  
- Kubelet  
- Security and permmisions: 
    - ServicaAccount
    - Role
    - ClusterRole
    - RoleBinding
    - ClusterRoleBinding
- Secrets & ConfigMaps


---

### Final Exercise:

- Write a deployment plan to serve a machine learning model using Kubernetes. Design your archtiecture in [draw.io](https://draw.io).  
- Your plan should include:
  - A container image for the model
  - How you would expose it (e.g., `Service` or `Ingress`)
  - How you would manage versioning or rollouts
  - How GPU usage would be scheduled (if applicable)
  - try deploying a local K8S cluster on your PC/VM (search the internet how to do it!) and try deploying it!

- Present it to your hofef, explaining:
  - What each component does (Pod, Deployment, etc.)
  - How this setup supports scalability and reliability
