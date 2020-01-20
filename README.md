---
comments: true
feedback: true
description: 'Learn how to use and configure the Jenkins role.'
repositories:
  - domain=Ansible Role Jenkins, repository=https://github.com/lordoftheflies/jenkins
  - domain=Ansible Role Jenkins, repository=https://gitlab.cherubits.hu/oss/ansible-galaxy-roles/ansible-role-jenkins
  - domain=Ansible Role Jenkins, repository=https://gitlab.com/lordoftheflies/ansible-role-jenkins
---

# Ansible Role: Jenkins

[![Build Status](https://travis-ci.org/lordoftheflies/ansible-role-jenkins.svg?branch=master)](https://travis-ci.org/lordoftheflies/ansible-role-jenkins)
[![Travis CI](http://img.shields.io/travis/lordoftheflies/ansible-role-jenkins/default.svg?style=flat)](http://travis-ci.org/lordoftheflies/ansible-role-jenkins/default)

[![Platform](http://img.shields.io/badge/platforms-debian%20/%20ubuntu-yellowgreen.svg?style=flat)](#)
[![Platform](http://img.shields.io/badge/platforms-debian%20/%20debian-yellowgreen.svg?style=flat)](#)
[![Platform](http://img.shields.io/badge/platforms-rhel%20/%20centos-yellowgreen.svg?style=flat)](#)
[![Platform](http://img.shields.io/badge/platforms-rhel%20/%20fedora-yellowgreen.svg?style=flat)](#)
[![Platform](http://img.shields.io/badge/platforms-archlinux%20/%20archlinux-yellowgreen.svg?style=flat)](#)
[![Platform](http://img.shields.io/badge/platforms-suse%20/%20opensuse-yellowgreen.svg?style=flat)](#)

## Description

[Ansible](https://www.ansible.com/) [Galaxy](https://galaxy.ansible.com/) Role for [Jenkins](https://jenkins.io/) installation and administering.

## Roadmap

* [ROADMAP.md](ROADMAP.md)

## References

* [Ansible Documentation](https://docs.ansible.com/)
* [Jenkins User Manual](https://jenkins.io/doc/)

## Requirements

* lordoftheflies.java

### Production

* Ansible

### For Local Testing

* [Vagrant](https://www.vagrantup.com/) - (Tested using version 2.1.1)
* Vagrant plugins:
  * [vagrant-disksize (0.1.2)](https://github.com/sprotheroe/vagrant-disksize)
  * vagrant-vbguest (0.15.2) - Recommended [vagrant-vbguest](https://github.com/cjsteel/vagrant-vbguest)
  * vai (0.9.3) - For testing with multiple vms [vagrant-plugin-vai](https://github.com/cjsteel/vagrant-plugin-vai) 
* [Virtual Box](https://www.virtualbox.org/)
  * Tested using Version 5.2.14 r123301 (Qt5.6.1) 

## Variables

<p>

<details>

<summary>Jenkins Version</summary>

#### Jenkins version

Version of Jenkins, which will be installed by the role.

</details>

</p>

<p>

<details>

<summary>Working Directory</summary>

#### Working Directory

Working directory for Jenkins installation.

</details>

</p>

### Variable Defaults

* [defaults/main.yml](defaults/main.yml) contains all of the required variables.

### Site Example

* [files/example.yml](files/example.yml) may contain an example entry.

## Testing

To test with all VM's defined in Vagrantfile run the following:

```bash
cd roles/ansible-role-jenkins
vagrant up
```

To run on a specific VM's
```bash
vagrant up xenial
```

### VM's tested with Vagrant and Virtualbox

pass, fail, untested

| Platform | Family | Distribution | Results  |
| :---: | :---: | :---: | :---: |
| Debian | Ubuntu | precise | untested |
| Debian | Ubuntu | trusty | untested |
| Debian | Ubuntu | xenial | pass |
| Debian | Ubuntu | bionic | pass |
| Debian | Ubuntu | disco | pass |
| Debian | Ubuntu | eon | pass |
| RHEL | CentOS | 6 | untested |
| RHEL | CentOS | 7 | untested |
| RHEL | Fedora | | untested |
| Arch | Archlinux |  | fail |
| Suse | OpenSUSE |  | fail |

## Authors and License

- [László Hegedűs](https://portal.cherubits.hu/) | [e-mail](mailto:laszlo.hegedus@cherubits.hu)

License: [Apache-2.0](LICENSE)
* ansible-role-jenkins generated using [galaxy-role-skeleton](https://github.com/cjsteel/galaxy-role-skeleton)
