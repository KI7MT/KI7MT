![Linux](https://img.shields.io/badge/Linux-Advanced-teal?style=flat-square)
![Bash](https://img.shields.io/badge/Bash-Advanced-teal?style=flat-square)
![Python](https://img.shields.io/badge/Python-Advanced-teal?style=flat-square)
![CSharp](https://img.shields.io/badge/CSharp-Intermediate-ffea00?style=flat-square)
![Java](https://img.shields.io/badge/Java-Intermediate-ffea00?style=flat-square)
![Go](https://img.shields.io/badge/Go-Learning-orange?style=flat-square)
![Scala](https://img.shields.io/badge/Scala-Learning-orange?style=flat-square)

## About

I'm an avid supporter of [Open Source Software][] and like working with most any flavor Linux / BSD / UX. I've been a Linux user dating back to the early [Slackware][] days. I've used Ubuntu since ~2005 ([5.04][]), [Ubuntu Member][] since 2013-ish, and [Launchpad Package Maintainter][] (off and on) since  2010. Over the years I've also used Red Hat, Fedora, CentOS. Currently using [Ubuntu 20.04][] as my home workstation, [Pop\!_OS][] for gaming, and [Oracle Linux][] (descendant of [RHEL][]) for enterprise work. I also have a fondness for rolling distributions such as [Arch][] and [Gentoo][]. [Alpine][] is my go-to distribution for most things container related, unless there is a reason to go in a different direction. Basically, I just like Linux, of any flavor !!

## Development Focus

My current language focus is on [Terraform][] and [Ansible][] for [Infastructure as Code][]. Cloud based tools of interest are centered on [Oracle Cloud Infastructure (OCI)], and [Nomad][] using [Docker][] or [LXC][] containers. I've rescently started learning / testing High-Availability discovery and secrets management using [Vault][] and [Consul][].

Coding projects getting the most attention are related to Big Data in Amateur Radio:

- [WSPR Analytics] - Exploring [WSPR][] / [WSPRDAEMON][] spots using Big Data Tools ([Scala][], [PySpark], and [Apache Arrow][])

## Home Lab

My current home-lab consists of a 16 core/32 thread virtualization node, and a few smaller 4 core/8 thread AMD V1605B SoC's ([GB-BSRE-1605][]) clusterd with the Type-1 Hypervisor [Proxmox][]. The network stack is fairly simple employing a Dual-WAN failover via [Netgate 3100][] and [pfSense][]. Core distribution is through a [USW-PRO-24 PoE][]. A 10GB aggregation switch ([US-XG-16][]) is used for wiring up storage and virtualization. Several smaller PoE switches power Wireless AP's, cameras, printers, IoT devices, etc. Network storage is [TrueNAS Core][] on a high-speed 14TB ZFS pool. For future storage and backup, I'm looking at the [Synology RS2421][] or the [iX-Systems][] [ix-1212i][], but that could change. 

<!--
- [JTSDK64 Tools Documentation][] Principal, and current author
- [JTSDK Founding Developer][] - Original Author
- [JTSDK@groups.io] - Owner, and community contributor
- [JTSDK Tools Gthub Project][] - Contributor
-->

<!-- Page Links-->
[Open Source Software]: https://opensource.com/resources/what-open-source
[Golang]: https://golang.org/
[WSPR Analytics]: https://github.com/KI7MT/wspr-analytics
[WSPR]: https://www.physics.princeton.edu/pulsar/k1jt/wspr.html
[WSJTX UDP REST API]: https://github.com/KI7MT/wsjtx-logapi-go
[WSJT-X]: https://www.physics.princeton.edu/pulsar/k1jt/wsjtx.html
[5.04]: http://old-releases.ubuntu.com/releases/
[Ubuntu Member]: https://wiki.ubuntu.com/KI7MT
[Spark]: https://spark.apache.org/
[Scala]: https://scala-lang.org/
[PySpark]: https://spark.apache.org/docs/latest/api/python/index.html
[Apache Arrow]: https://arrow.apache.org/
[Slackware]: https://en.wikipedia.org/wiki/Slackware
[Launchpad Package Maintainter]: https://launchpad.net/~ki7mt
[JTSDK64 Tools Documentation]: https://jtsdk.github.io/jtsdk64-tools/
[JTSDK Founding Developer]: https://sourceforge.net/projects/jtsdk/
[JTSDK@groups.io]: https://groups.io/g/JTSDK
[Knoppix]: http://knoppix.net/
[Arch]: https://archlinux.org/
[Arch Linux]: https://archlinux.org/
[Gentoo]: https://www.gentoo.org/
[JTSDK Tools Gthub Project]: https://github.com/JTSDK
[WSPRDAEMON]: http://wsprdaemon.org/
[Alpine]: https://www.alpinelinux.org/
[HashiCorp Vagrant]: https://www.vagrantup.com/
[Docker]: https://www.docker.com/
[Scala]: https://scala-lang.org/
[Oracle Cloud Infastructure (OCI)]: https://www.oracle.com/cloud/
[Micronaut]: https://micronaut-projects.github.io/micronaut-oracle-cloud/latest/guide/
[GraalVM]: https://www.graalvm.org/
[Java]: https://www.oracle.com/java/
[Kubernetes]: https://kubernetes.io/
[Nomad]: https://www.nomadproject.io/
[Proxmox]: https://www.proxmox.com/en/
[pfSense]: https://www.pfsense.org/
[US-XG-16]: https://store.ui.com/collections/unifi-network-switching/products/unifi-switch-16-xg
[Switch Pro 24 PoE]: https://store.ui.com/collections/unifi-network-switching/products/usw-pro-24-poe
[TrueNAS Core]: https://www.truenas.com/truenas-core/
[LXC]: https://linuxcontainers.org/lxc/introduction/
[GB-BSRE-1605]:https://www.gigabyte.com/us/Mini-PcBarebone/GB-BSRE-1605-rev-10#kf
[USW-PRO-24 PoE]: https://store.ui.com/collections/unifi-network-switching/products/usw-pro-24-poe
[Ubuntu 20.04]: https://ubuntu.com/
[Oracle Linux]: https://www.oracle.com/linux/
[RHEL]: https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux
[Pop\!_OS]: https://pop.system76.com/
[Synology RS2421]: https://www.synology.com/en-us/products/RS2421+
[Netgate 3100]: https://shop.netgate.com/products/3100-base-pfsense
[Consul]: https://www.consul.io/
[Vault]: https://www.vaultproject.io/
[ix-1212i]: https://www.ixsystems.com/ix-server-family/rackmount-servers/ix-1212i/
[iX-Systems]: https://www.ixsystems.com/
[Terraform]: https://www.terraform.io/
[Ansible]: https://www.ansible.com/
[Infastructure as Code]: https://developer.oracle.com/infrastructure-as-code/

<!--
**KI7MT/KI7MT** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
