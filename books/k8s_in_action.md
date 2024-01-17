### Chapter 1: Introduction
- Monolithic apps are easier to deploy, but harder to maintain over time and
sometimes impossible to scale.
- Microservices-based application architectures allow easier development of each
component, but are harder to deploy and configure to work as a single system.
- Linux containers provide much the same benefits as virtual machines, but are
far more lightweight and allow for much better hardware utilization.
- Docker improved on existing Linux container technologies by allowing easier and
faster provisioning of containerized apps together with their OS environments.
- Kubernetes exposes the whole datacenter as a single computational resource
for running applications.
- Developers can deploy apps through Kubernetes without assistance from
sysadmins.
- Sysadmins can sleep better by having Kubernetes deal with failed nodes automatically.

### Chapter 2: First steps with Docker and Kubernetes

- Working with [minikube](https://minikube.sigs.k8s.io/docs/start/)
- Pull and run any publicly available container image
- Package your apps into container images and make them available to anyone by pushing the images to a remote image registry
- Enter a running container and inspect its environment
- Configure an alias and tab completion for the kubectl command-line tool
- List and inspect Nodes, Pods, Services, and ReplicationControllers in a Kubernetes cluster
- Run a container in Kubernetes and make it accessible from outside the cluster
- Have a basic sense of how Pods, ReplicationControllers, and Services relate to one another
- Scale an app horizontally by changing the ReplicationController’s replica count
- Access the web-based Kubernetes dashboard on Minikube

