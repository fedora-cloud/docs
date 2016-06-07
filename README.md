# Fedora Cloud Documentation

## NOTE: ALL ITEMS HERE SHOULD CURRENTLY BE CONSIDERED DRAFT

Here in lies Fedora's Cloud Documentation, the goal of this github repository is
to host documentation (regardless of markup language) as well as a list of
externally hosted Cloud related Documentation.

# Pull Requests
If there are any documents that you would like to see updated or created, please
issue a pull request and we will gladly accept it.

New docs should go into `docs` dir.

# External Links

In this section of the README we will maintain a list of documentation that is
hosted external to this git repository. As time goes on we plan to merge these
documentation efforts but for now we need to have a single location that can
index currently available content as well as create new content.

* [Fedora Cloud User Guide](http://fedoracloud.readthedocs.io/en/latest/)
* [Fedora Cloud Guide
  DRAFT](https://docs.fedoraproject.org/en-US/Fedora_Draft_Documentation/0.1/html/Cloud_Guide/index.html)

# Wishlist

These are docs we would like to see written

* What is Fedora Cloud?
* What is Atomic / Atomic Host?
    * Why is this interesting, why should I as an user care?
    * How do I get up and running with Fedora Atomic Host?
        * on bare metal
        * on AWS
        * on other clouds/VMs
* How do I run apps and services on Fedora Atomic Host?
    * What is a super priv container?
    * What is an atomic-app?
    * How do I create one?
* How do I do "traditional" sysadmin things in Atomic Host?
    * rsyslog Super Priv Container
    * nginx/ httpd as dev server
    * Ansible-container ?
* Single-Host
    * Multi-Host Container Orchestration:
    * OpenShift/Kubernetes/Deis/etc
    * Mesos
    * Docker Swarm
* IaaS Cloud Provider Specific Guides (both Atomic and regular Fedora)
    * AWS
    * Digital Ocean
    * Linode
* Vagrant
    * what it is, how to use it
    * using Vagrant to deploy to cloud providers
* Ansible
* docker examples from (Fedora Dockerfiles)[https://github.com/fedora-cloud/Fedora-Dockerfiles]
    * These will eventually be converted into DistGit when the Docker Layered Image Build System is eventually available
* Building Images
    * How do I build images based on Fedora base images?
    * What is the layered image build service, and how do I use it?
    * systemd in containers?

# Licensing

To make licensing easier, license headers in the source files will be
a single line reference to Unique License Identifiers as defined by
the [Linux Foundation's SPDX project](http://spdx.org/).

For example, in a source file the full "GPL v2.0 or later" header text will be
replaced by a single line:

    SPDX-License-Identifier:    GPL-2.0+

Or alternatively, in a source file the full "CC-BY-SA-4.0" header text will be
replaced by a single line:

    SPDX-License-Identifier:    CC-BY-SA-4.0

the license terms of all files in the source tree should be defined
by such License Identifiers; in no case a file can contain more than
one such License Identifier list.

If a `SPDX-License-Identifier:` line references more than one Unique
License Identifier, then this means that the respective file can be
used under the terms of either of these licenses, i. e. with

    SPDX-License-Identifier:    GPL-2.0+    LGPL-2.1+

All SPDX Unique License Identifiers available [here](http://spdx.org/licenses/).
