# Attacking Docker Containers - Scenarios

In this section we will be attacking the containers to gain access to the host system, data and assets.

* Attacking container capabilities
* Attacking insecure volume mounts in containers
* Attacking runtime misconfigurations
* Exploiting docker secrets misconfiguration

`Docker Escape` is the term used to define vulnerabilities, weaknesses and their exploitation technique that allows an attacker to bypass the various restrictions enforced by the container runtime.

An escape happens when an attacker having access to execute arbitrary command inside a container is able to access or execute commands on the host system, outside the container namespace restrictions.

> For this section, we assume that an attacker has already gained access to execute commands inside a container by exploiting some vulnerability in app deployed in the container.
