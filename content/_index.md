---
date: 2016-03-08T21:07:13+01:00
title: DevSecOps Studio 
type: index
next: /getting-started/
weight: 10
---

## Welcome to DevSecOps Studio Project!

DevSecOps Studio is one of its kind, self contained DevSecOps environment/distribution to help individuals in learning DevSecOps concepts. It takes lots of efforts to setup the environment for training/demos and more often, its error prone when done manually. DevSecOps Studio is easy to get started, mostly automatic and battle tested during our [Free Practical DevSecOps Course](https://www.teachera.io/devsecops-course/)

DevSecOps Studio project aims to reduce the time to bootstrap the environment and help you in concentrating on learning/teaching DevSecOps practices.

![](/images/appsec-pipeline.png)

## Features

- Easy to setup environment with just one command “vagrant up”
- Teaches Security as Code, Compliance as Code, Infrastructure as Code
- With built-in support for CI/CD pipeline
- OS hardening using ansible
- Compliance as code using Inspec
- QA security using ZAP, BDD-Security and Gauntlt
- Static tools like bandit, brakeman, windbags, gitrob, gitsecrets
- Security Monitoring using ELK stack. 


> **Note:**

> - We use this repo as companion to our Free [Practical DevSecOps course](https://www.teachera.io/devsecops-course/).

> - If you wish to join our free course, please click on __Join the course__ in the above link.


## Quick start

Install [Vagrant](https://www.vagrantup.com/downloads.html), [Virtualbox](https://www.virtualbox.org/wiki/Downloads), [Ansible](http://docs.ansible.com/ansible/latest/intro_installation.html#installation) and Follow the below steps.

```bash
# Download the code
$ git clone https://github.com/teacheraio/DevSecOps-Studio.git && cd DevSecOps-Studio

# Download the ansible dependency roles
$ ansible-galaxy install -r requirements.yml -p provisioning/roles

# Setup the environment, takes an hour or less based on your internet speed.
$ vagrant up
```

Go grab some coffee while DevSecOps Studio does its job.

Yes, that's it, you just setup entire DevSecOps environment with three commands.

See the [getting started guide]({{< relref "getting-started/index.md" >}}) for instructions how to get
it up and running.

## Acknowledgements

Last but not least a big thank you to [Hari K](@vhsunny1) for providing continuous feedback during this project. 

Furthermore, DevSecOps Studio uses some of the ansible roles from [Jeff](https://github.com/geerlingguy)


