Ansible-Kubernetes Role
=========

A simple Ansible role for deploying and initialize your K8s cluster on Linux servers.

Requirements
------------

- At least you need 1 server for master and 1 server for worker
- Each of your server must have following resources: 2 vCPUs, 2 GB RAM
- Ansible v2.7 or higher on your local computer which will execute Ansible-playbooks

Role Variables
--------------

`kubeadm_version` # versisn of kubeadm to install
`kubectl_version` # version of kubectl to install
`kubelet_version` # version of kubelet to install

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
    - hosts: servers
      roles:
         - { role: ansible-kubernetes.yml }
```
