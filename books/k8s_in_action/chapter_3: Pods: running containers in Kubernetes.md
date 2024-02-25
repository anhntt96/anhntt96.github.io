#### UNDERSTANDING THE PARTIAL ISOLATION BETWEEN CONTAINERS OF THE SAME POD
- Because all containers of a pod run under the same Network and UTS namespaces
(we’re talking about Linux namespaces here), they all share the same hostname and
network interfaces. Similarly, all containers of a pod run under the same IPC namespace
and can communicate through IPC. In the latest Kubernetes and Docker versions, they
can also share the same PID namespace, but that feature isn’t enabled by default.

#### UNDERSTANDING HOW CONTAINERS SHARE THE SAME IP AND PORT SPACE
- This means processes running in containers of the same pod need to take care not to bind to the same port numbers or they’ll run into port conflicts.

### Creating pods from YAML or JSON descriptors
3 important sections:
- *Metadata* includes the name, namespace, labels, and other information about
the pod.
- *Spec* contains the actual description of the pod’s contents, such as the pod’s containers, volumes, and other data.
- *Status* contains the current information about the running pod, such as what
condition the pod is in, the description and status of each container, and the
pod’s internal IP and other basic info.


```
apiVersion: v1 
kind: Pod
metadata:
  name: kubia-manual
spec:
  containers:
  - image: luksa/kubia
    name: kubia
    ports:
    - containerPort: 8080
      protocol: TCP
```
- Creating, running, and stopping pods
- Organizing pods and other resources with labels
- Performing an operation on all pods with a specific label
- Using namespaces to split pods into non-overlapping groups
- Scheduling pods onto specific types of worker nodes