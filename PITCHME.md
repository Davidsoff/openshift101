#Openshift 101
###By : David Soff

+++

#Before we start
Please clone the following git repository if you want to follow along with the hands-on excercises.

```https://github.com/Davidsoff/openshift101.git```

---

#Content
- 5-minute Dockerfile refresher
- What is Openshift
- Why we chose Openshift
- Openshift Concepts

---

# Dockerfile

+++?code=ex1/Dockerfile
@[1](base image)
@[3](set user, does nothing in this case as user is already root)
@[5](copies files into layer, prefer this over ADD)
@[7](Exposes a port for mapping)

---

