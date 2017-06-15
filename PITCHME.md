# OpenShift 101
By: David Soff

+++

# Before we start
Please clone the following git repository if you want to follow along with the hands-on exercises.

```https://github.com/Davidsoff/openshift101.git```

---

# Content
- 5-minute Dockerfile refresher
- What is OpenShift
- Why we chose OpenShift
- OpenShift Concepts

---

# Dockerfile

+++?code=ex1/Dockerfile
@[1](Base image)
@[3](Sets user)
@[5](Copies files into container)
@[7](Exposes a port for mapping)

---

# OpenShift

- "Enterprise Kubernetes"
- Made by RedHat
- Opensource

+++

# Enterprise Kubernetes?

+++

# Kubernetes
- Container orchestrator
- Open-sourced by Google based on Borg
- Container scheduling and monitoring
- project by CNCF
- and much more!

Note: CNCF = Cloud Native Computing Foundation
+++

# Extra in OpenShift
- Builds |
- Pipelines |
- Role Based Acces Control |
- More fancy dashboard |

Note: RBAC is now a Kubernetes Beta

---

# Choosing OpenShift

+++

# Competition
- Kubernetes |
- Docker Swarm |
- Apache Mesos |

+++

# Kubernetes
- Has a big community and is supported by CNCF
- Is missing some nice to have features like RBAC and Builds

+++

# Docker Swarm
- Integrated in Docker Core
- Is missing features like auto-scaling and namespacing

+++

# Apache Mesos
- Very flexible
- High barrier to entry

+++

# So why OpenShift?

Because it's geared towards Developer Self-Service

---

# Openshift concepts
- Containers and images |
- Pods and services |
- Projects and users |
- Builds and image streams |
- Deployments |
- Routes |
- Templates |

---

# Containers and images

Note: building blocks of all your applications
Note: push built images to the OpenSift registry

---

# Pods and services

+++

# Pods
- Unit of scaling
- Unit of deployment
- One or more containers

Note: Pod is smallest deployable unit in OpenShift
Note: Pod can contain one or more containers
Note: containers in pods guaranteed to run on same host

+++

# Services
- Internal load balancer
- Enables High-Availability and rolling deploys

Note: do pods and services exercise

---

# Users and projects

+++

# Users
There are three user types:

- Regular users
- System users
- Service accounts

Note: service accounts are special users associated with an account, like deployer and builder

+++

# Projects
- Scope resources
- Can constrain resource usage
- Have access policies

---

# Image streams and builds

+++

# Image streams

+++

# Builds
(Usually) transforms source code into an image using a build strategy

Openshift has four strategies:

- Docker build
- Source-to-image build
- Custom build
- Pipeline build 

+++

# Source-to-image

uses builder image to produce a ready to run Docker image

Note: do s2i exercise

+++

# Pipelines

Can be used to implement sophisticated workflows
Use a Jenkinsfile for configuration

Note: do pipeline-cd exercise

---

# Deployments
- Start pods
- Can be automatically triggered
- Manage transistion between versions

Note: apply recreate-strategy to pipeline exercise

---

# Routes
- Expose services on a URL
- Can do traffic sharding
- Can be used as SSL terminators

Note: create route for pipeline exercise

---

# Templates
> A template describes a set of objects that can be parameterized and processed to produce a list of objects for creation by OpenShift.

Note: we've been using these in the exercises.

---

# Thank you!

---

# Any questions?