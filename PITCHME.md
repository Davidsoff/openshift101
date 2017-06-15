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

---

# Pods and services

---

# Projects and users

---

# Builds and image streams

---

# Deployments

---

# Routes

---

# Templates

---

# Thank you!

---

# Any questions?