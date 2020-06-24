# Development Env and Vagrant 101

This repo is a vagrant machine that instals nginx as well as expose it on an ip and host name.

#### Installation

To get this box running:
1. clone the reproducible
2. make sure you are on the root of the project and can see the vagrantfile 3. then run:
```bash
vagrant up
```

Now you can see nginx running on 2 locations:
- ip: 192.168.10.100
- development.local/

#### What is an environment?
An environment is a location where code runs and data lives.

Github is not an environment really, maybe Github pages.

Your machine is an environment because code runs and you develop software and web apps and other apps.

What environments are there?

Developments:
where you write your code, Py, Sql, Html - i.e. computer
Testing:
external, has its own tools and infrastructure that runs the code
Production:
Code pipelines: move between the environments.

Testing: ensures functionality and quality of the website.

Objective: increase speed of learning and developing -> increase feedback loops -> increase innovation.

#### Dev environment

A set of processes and tools that are used to develop a source code or program.

#### 4 pillars of DevOps

Ease of use: everyone on the team will use this, which is why documentation is important.
Flexibility: things change at incredible rate, you don't want to change that fast but adapt accordingly.
Robustness: we need 100% uptime, fast and robust deployment
Cost: cost of downtime, cost of slow innovation, cost of time to market, cost of infrastructure

#### DevOps problems and solutions

"It's working on my computer" - this is the main issue in DevOps, to avoid this you must standardise the environment.

## Vagrant & Virtual Box

### Vagrant

Vagrant enables users to create and configure lightweight, reproducible and portable development environments, e.g. VirtualBox, KVM, Docker.

### Virtual Box

Developed by Oracle Corporation, VirtualBox is a free and open-source hosted hypervisors for x86 virtualization. It allows users and administrators to easily run multiple guest operating systems on a single host.  

### Package manager
Package manager system is a collection of software tools that automates the process of installing, upgrading, configuring and removing computer programs for a computer's operating system in a consistent manner.

## what is python's package manager?
Python Package Manager (PyPM) - pip


## what is ubuntu's package manager?
 Debian Package Management System, Red Hat Package Manager, Pacman Package Manager, Zypper Package Manager, Portage Package Manage

## Steps:
vagrant init ubuntu/xenial64

vagrant up

put console.log in gitignore

vagrant ssh

sudo apt-get update -y

sudo apt-get install nginx -y

sudo systemctl start nginx
