# Network Programmability & Automation
### Light the New World
2017.03.06

This was put together as a form of tracking my path through the network automation jungle.  The choice of tools to learn is mostly environment based and as most of the customers I work for are Cisco based with a mix of firewalls/loadbalancers I am personally working through Python + netmiko & ciscoconfigparse for simple stuff and will be adding Ansible to the mix. I am using Cisco's VIRL as my test network. VIRL has an API too, it would be nice to able to completely automate the build and configuration of the VIRL test environment...

Originally started as an URL dump and as a GIT practice project. Most comments are cribbed from the source site or
  https://en.wikipedia.org/wiki/Comparison_of_open-source_configuration_management_software

#### March update
Trying to cull dead links & new topics.
#### Feb update
A new year and I'm making this a little more focused dropping Chef, Puppet and Salt.

## teaser
* http://automation.ipspace.net/Example:Using_Ansible_Playbooks_with_Cisco_VIRL


## Linux Cheat Sheet:
A little UNIX knowledge helps...
  https://fosswire.com/post/2007/08/unixlinux-command-cheat-sheet/

## GIT
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed & efficiency. [it is hard to get your head wrapped around how git works]
* https://git-scm.com/downloads
* https://desktop.github.com/ GUI + shell or powershell interface [I use the shell version]
* http://rogerdudler.github.io/git-guide
* https://git-scm.com/book/en/v2
* https://www.codeschool.com/ Codeschool has a free introduction GIT lesson (learn by doing)

## Network automation blogs:
* https://jedelman.com/          @jedelman8
* https://pynet.twb-tech.com/    @kirkbyers [netmiko]
* https://networklore.com/       Patrick Ogenstad
* http://keepingitclassless.net/ @mierden  [ToDD]
* http://ipSpace.net/            @ioshints Ivan Pepelnjak [web seminars as well]
* http://packetpushers.net/      lots of blogs and podcasts...
* https://sreeninet.wordpress.com
* https://codingnetworker.com    Henry Ölsner

## Network automation training:
* http://networktocode.com/	Jason Edelman's company for training + labs [also join his slack group here]
* http://ipSpace.net/ Ivan Pepelnjak's company with many (live/recorded) web seminars in subscription or buy options

## Cisco Network Programmability and DevOps
* https://learninglabs.cisco.com/tracks/netprog-eng
* https://learninglabs.cisco.com/tracks/devnet-express-dna
* https://developer.cisco.com/site/networking/ DNA starting point on DevNet
* https://communities.cisco.com/docs/DOC-71197 Configure ASA ACL's with APIs

## Cisco Training & Certification for Network Programmability
Has some (limited) free trial chapters.
* https://learningnetwork.cisco.com/community/certifications/network-programmability/design-and-implementation
* https://learningnetworkstore.cisco.com/network-programmability-specialists
* https://learningnetworkstore.cisco.com/on-demand-e-learning/programming-for-network-engineers-prne-v1-0-elt-prne-v1-0-020276
* https://www.ciscolearningsystem.com Course site for above has sandbox for labs

## Python
Search the O'Reilly website for the free eBooks "A Whirlwind Tour of Python" & "How to Make Mistakes in Python" (worth reading the first chapter or so of Mistakes before installing any version of Python)
* https://www.python.org
* https://www.continuum.io/downloads Anaconda: Python + development environment (I use this)
* https://developers.google.com/edu/python is the website of Google’s (free) Python course that I first watched
* https://www.codeschool.com/ Codeschool has a free introduction Python lesson (my second pick)
* https://www.dabapps.com/blog/introduction-to-pip-and-virtualenv-python/
* https://training.talkpython.fm also home to a good python podcast on the main site talkpython.fm
* http://nedbatchelder.com/text More advanced; PyCon talks good! (free)
* https://pythonprogramming.net/introduction-to-python-programming (free)
* https://pythonprogramming.net/introduction-intermediate-python-tutorial (free)

#### more advanced python stuff
* https://www.fullstackpython.com/ pushing your knowledge further
* https://awesome-python.com/ Curated list of frameworks, libraries, software and resources.

#### Netmiko
An open-source Python library that simplifies SSH management to network devices. The library is based on the Paramiko SSH library.
* https://pynet.twb-tech.com/
* [Packet Pushers #270 Automation with Python & Netmiko](http://packetpushers.net/podcast/podcasts/show-270-design-build-9-automation-python-netmiko/)

#### ciscoconfparse
ciscoconfparse is a Python library, which parses through Cisco IOS-style configurations
* http://www.pennington.net/py/ciscoconfparse
* https://codingnetworker.com/2016/06/parse-cisco-ios-configuration-ciscoconfparse
  I used this to dismantle ACE20 loadbalancer configurations into individual farms (with a little manual checking afterwards)

#### TextFSM
TextFSM is a Python module that implements a template based state machine for parsing semi-formatted text.
* https://github.com/google/textfsm
* http://www.oznetnerd.com/category/automation/textfsm
* https://codingnetworker.com/2015/08/parse-cli-outputs-textfsm

#### pip installs: netaddr & ipaddress
IP address & network manipulation
* https://pythonhosted.org/netaddr/installation.html
* https://pythonhosted.org/netaddr/tutorial_01.html
* https://docs.python.org/3/howto/ipaddress.html
* https://docs.python.org/dev/library/ipaddress.html

#### JINJA2
Jinja2 is a full featured template engine for Python.
* http://jinja.pocoo.org

#### Trigger
Trigger is a Python framework and suite of tools for interfacing with network devices and managing network configuration and security policy. (similar to netmiko/paramiko? haven't looked deep at this yet and it's not high on the list of things to do)
* https://trigger.readthedocs.io/en/latest/overview.html

#### NAPALM (Network Automation and Programmability Abstraction Layer with Multivendor support)
NAPALM is a Python library that implements a set of functions to interact with different network device Operating Systems using a unified API. Has gone native in Ansible & Salt with offical modules (see notes in doc & on GIThub site).
* https://napalm.readthedocs.io/en/latest/index.html
* https://github.com/napalm-automation/napalm
* https://pynet.twb-tech.com/blog/automation/napalm-ios.html

#### YAML: YAML Ain't Markup Language
YAML is a human friendly data serialization standard for all programming languages.
* http://yaml.org/
* http://docs.ansible.com/ansible/YAMLSyntax.html
* http://www.yaml.org/spec/1.2/spec.html
* http://pyyaml.org/ YAML implementations for Python
Check the validity of your YAML and errors + get a nice clean UTF-8 version of it.
* http://www.yamllint.com

### JSON
(JavaScript Object Notation) is a lightweight data-interchange format.
* http://json.org/

### YANG - Data Modeling Language.
* https://developer.cisco.com/site/ydk/
* https://developer.cisco.com/site/ydk/documents/overview/
* https://communities.cisco.com/community/developer/ydk


### Postman
Roll your own API...
https://www.getpostman.com

### Zero to API in 4 Minutes
Blog post covering build your own API uses flask & swagger (python stuff)
https://cidrblock.github.io/zero-to-api-in-4-minutes.html


## Open-source Configuration Management Software
* https://en.wikipedia.org/wiki/Comparison_of_open-source_configuration_management_software

Good podcasts on these topics on Packet Pushers (list not up to date):
* http://packetpushers.net/podcast/podcasts/show-176-intro-to-python-automation-for-network-engineers
* http://packetpushers.net/podcast/podcasts/show-198-kirk-byers-network-automation-python-ansible
* http://packetpushers.net/podcast/podcasts/show-270-design-build-9-automation-python-netmiko
* http://packetpushers.net/podcast/podcasts/datanauts-034-automate-packets
* http://packetpushers.net/podcast/podcasts/pq-show-99-netmiko-napalm-network-automation

One engineers view of Salt & Ansible, useful for an overview of both:
* http://jensrantil.github.io/salt-vs-ansible.html

### ANSIBLE
Combines multi-node deployment, ad-hoc task execution, and configuration management in one package. Manages nodes over SSH and requires python (2.4 or later) to be installed on them. Modules work over JSON and standard output and can be written in any language. Uses YAML to express reusable descriptions of systems.
* https://www.ansible.com/
* https://www.ansible.com/quick-start-video
* https://www.ansible.com/network-automation
* http://docs.ansible.com/ansible/index.html
* https://networklore.com/ansible-getting-started/
* http://jpmens.net/2012/06/06/configuration-management-with-ansible/
* http://www.oreilly.com/webops-perf/free/network-automation-with-ansible.csp
* https://galaxy.ansible.com/Juniper/junos/
* http://docs.ansible.com/ansible/intro_networking.html
* http://docs.ansible.com/ansible/ios_config_module.html
* https://cidrblock.github.io/ansible-playbook-from-the-ground-up.html

LEARNING LAB:
* https://www.turnkeylinux.org/ansible **Ansible on a VM**
* https://github.com/turnkeylinux-apps/ansible/blob/master/docs/usage.rst


### SALT
Salt started out as a tool for remote server management. As its usage has grown, it has gained a number of extended features, including a more comprehensive mechanism for host configuration. This is a relatively new feature facilitated through the Salt States component. With the traction that Salt has gotten in the last bit, the support for more features and platforms might continue to grow.
* https://saltstack.com/community/ <-best starting point
* https://blog.talpor.com/2014/07/saltstack-beginners-tutorial/

LEARNING LAB:
**uses Vagrant on Virtual Box to setup the lab ie automation in action**
* https://docs.saltstack.com/en/getstarted/fundamentals/index.html


##Mixed stuffs:

### RBFS (REST based file-server)
RBFS provides a RESTful, JSON based, interface to a file system.
* https://github.com/cidrblock/RBFS

### VAGRANT
Vagrant is computer software that creates and configures virtual development environments. It can be seen as a higher-level wrapper around virtualization software such as VirtualBox, VMware, KVM and Linux Containers (LXC), and around configuration management software such as Ansible, Chef, Salt, and Puppet.
* https://www.vagrantup.com/
* http://www.vagrantbox.es/
* http://www.cyberciti.biz/cloud-computing/use-vagrant-to-create-small-virtual-lab-on-linux-osx

### VirtualBox
Free equiv to VMware Workstation Pro and you can create desktop shortcuts to start VMs directly
* https://www.virtualbox.org/wiki/Downloads
* https://www.virtualbox.org/manual/ch06.html

How to hook your VMware Workstation VM and Virtual Box VM together (to manage VIRL devices etc)
Sadly won't work with VMware Player...
* http://www.sysprobs.com/setup-network-virtualbox-vmware-virtual-machines

### VMware stuff:
* https://rednectar.net/2011/07/20/vmware-interfaces-tutorial/
* http://www.virtualizationadmin.com/articles-tutorials/vmware-server-workstation-player-articles/understanding-virtual-networking-vmware-workstation-9.html

### Turnkey Linux
VMs/ISOs/containers for various purposes:
* https://www.turnkeylinux.org/
* https://www.turnkeylinux.org/core
* https://www.turnkeylinux.org/ansible

## ToDD
A highly extensible framework for distributed capacity and connectivity testing (Testing on Demand....Distributed!)
* https://github.com/toddproject/todd
* https://www.youtube.com/watch?v=ZIykHS5RoNM
* http://packetpushers.net/podcast/podcasts/pq-show-81-network-testing-todd

## Front ends
front your own API/montioring/config system?
*  https://www.airpair.com/python/posts/django-flask-pyramid

###     DJANGO
Django is a high-level Python Web framework that encourages rapid development and clean, pragmatic design.
* https://www.djangoproject.com/
* https://docs.djangoproject.com/en/1.9/intro/tutorial01/

###     Flask
similar purpose to Django but simpler and included in anaconda by default
* http://flask.pocoo.org/
* https://pypi.python.org/pypi/Flask/0.11


