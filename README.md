# Ansible Role: Jenkins

## Status

[![Build Status](https://travis-ci.org/lordoftheflies/ansible-role-jenkins.svg?branch=master)](https://travis-ci.org/lordoftheflies/ansible-role-jenkins)
[![Travis CI](http://img.shields.io/travis/lordoftheflies/ansible-role-jenkins/default.svg?style=flat)](http://travis-ci.org/lordoftheflies/ansible-role-jenkins/default)

[![Platform](http://img.shields.io/badge/platforms-debian%20/%20ubuntu-lightgrey.svg?style=flat)](#)
[![Platform](http://img.shields.io/badge/platforms-debian%20/%20debian-lightgrey.svg?style=flat)](#)
[![Platform](http://img.shields.io/badge/platforms-rhel%20/%20centos-lightgrey.svg?style=flat)](#)
[![Platform](http://img.shields.io/badge/platforms-rhel%20/%20fedora-lightgrey.svg?style=flat)](#)
[![Platform](http://img.shields.io/badge/platforms-archlinux%20/%20archlinux-lightgrey.svg?style=flat)](#)
[![Platform](http://img.shields.io/badge/platforms-suse%20/%20opensuse-lightgrey.svg?style=flat)](#)

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

### defaults/main.yml

* [defaults/main.yml](defaults/main.yml) contains all of the required variables.

### project_name/site.yml example

* [example.yml](files/example.yml) may contain an example entry.

## Testing

To test with all VM's defined in Vagrantfile run the following:

```shell
cd roles/ansible-role-jenkins
vagrant up
```

To run on a specific VM's
```shell
vagrant up xenial
```

### VM's tested with Vagrant and Virtualbox

pass, fail, untested

| Platform | Family | Distribution | Results  |
| :--- | :--- | :--- | :--- |
| Debian | Ubuntu | precise | [ ] |
| Debian | Ubuntu | trusty | [ ] |
| Debian | Ubuntu | xenial | [x] |
| Debian | Ubuntu | bionic | [ ] |
| Debian | Ubuntu | disco | [ ] |
| Debian | Ubuntu | eon | [x] |
| RHEL | CentOS | 6 | [ ] |
| RHEL | CentOS | 7 | [ ] |
| RHEL | Fedora | | [ ] |
| Arch | Archlinux |  | [ ] |
| Suse | OpenSUSE |  | [ ] |

## Authors and License

- [László Hegedűs](https://portal.cherubits.hu/) | [e-mail](mailto:laszlo.hegedus@cherubits.hu)

License: [Apache-2.0](LICENSE)


* ansible-role-jenkins generated using [galaxy-role-skeleton](https://github.com/cjsteel/galaxy-role-skeleton)
