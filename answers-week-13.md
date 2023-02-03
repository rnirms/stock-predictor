## Interview Readiness 
* <i> What does it mean to create a Docker image and why do we use Docker images? </i>

A Docker image is a pre-built environment to run an application. It includes all the necessary files, packages and configurations needed to run the application. 

Docker images are used by developers to package the applications and their dependencies into a single unit, so that they can be shared and deployed easily across various environments, in a consistent manner irrespective of the host environment. 

* <i> Please explain what is the difference from a Container vs a Virtual Machine? </i>

Both container and virtual machine (VM) provide virtual environments to run applications. But there are some key differences. Container isolates the application only at the process level, while sharing the OS and resources of the host environment. For instance Docker uses its runtime to interact with host OS. VMs on the other hand, are fully isolated from the host system by creating their own operating system, and utilising their own resources. So VMs are bulkier and therefore, less scalable, take longer to startup and less portable than containers.

* <i> What are 5 examples of container orchestration tools (please list tools)? </i>

Kubernetes; OpenShift; Mesos, Docker Swarm; AWS: Elastic Kubernetes Service, EC2 Container Service, Fargate; Google: container engine, cloud run; Azure: kubernetes service, managed openshift service, container instances

* <i> How does a Docker image differ from a Docker container? </i>

A Docker image is the blueprint to create Docker containers. The image is created with instructions in a Dockerfile. The container is a running instance of the Docker image. For the same Docker image, we can run multiple instances. 
