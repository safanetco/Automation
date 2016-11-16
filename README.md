# Network Programmability & Automation 
2016.11.14 - Light the New World

Basically a URL dump. Most comments are cribbed from the source site or 
  https://en.wikipedia.org/wiki/Comparison_of_open-source_configuration_management_software

This was put together as a form of tracking my path through the Automation Jungle.

Although the choice of tools to learn is mostly environment based, as most of the customers I work for are Cisco based with a mix of firewalls/loadbalancers I'm working through Python 2.7 + netmiko & ciscoconfigparse for simple stuff and adding Ansible. The plan is to build an Ansible VM and connect it to Cisco's VIRL as a test system. 

I note that VIRL has an API too. It would be nice to be able to get Vagrant to build and preconfigure my Ansible VM to be able to playbook the VIRL configuration as well as the VIRL simulations.


### Linux Cheat Sheet:
  https://fosswire.com/post/2007/08/unixlinux-command-cheat-sheet/

## GIT
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed & efficiency. [Oh that sounds so cute... but it is hard to get your head wrapped around]
* https://git-scm.com/downloads
* http://rogerdudler.github.io/git-guide/
* https://git-scm.com/book/en/v2
* Codeschool has a free introduction GIT lesson

## Network programming blogs:
* https://sreeninet.wordpress.com/ 
* https://codingnetworker.com/ 
* http://packetlife.net/ 
* https://jedelman.com/           @jedelman8 
* https://pynet.twb-tech.com/     @kirkbyers  
* http://keepingitclassless.net/  @mierden 

## Cisco Network Programmability and DevOps Learning Map - Foundations
https://communities.cisco.com/docs/DOC-66387
  links out to training sites some of which are free (including CodeSchool)

### Stuff I'm still getting around to adding or looking for good sources:
* NETCONF 
* YANG 
* JINJA2 
* JSON 
* REST API 
* ToDD [& influxdb] 

## LANGUAGES:

### Python
* https://www.python.org/
* https://www.continuum.io/downloads Anaconda
* https://developers.google.com/edu/python/ is the website of Google’s (free) python course
* https://training.talkpython.fm/ also home to a good python podcast
* http://nedbatchelder.com/text/ PyCon talks good! 
* Search the O'Reilly website for the free eBooks "A Whirlwind Tour of Python" & "How to Make Mistakes in Python"

###     PEP8
Formatting standard for Python - nice except for 80 char line lengths... forget it I'll try keep them under 100 instead.

###     Netmiko
An open-source Python library that simplifies SSH management to network devices. The library is based on the Paramiko SSH library. 
* https://pynet.twb-tech.com/
* Podcast - Packet Pushers #270 Automation with Python & Netmiko
    
###     ciscoconfparse 
ciscoconfparse is a Python library, which parses through Cisco IOS-style configurations
  Used this to dismantle ACE20 loadbalancer configurations into individual farms (with a little manual checking afterwards)
* http://www.pennington.net/py/ciscoconfparse  

###     pip installs: netaddr, ipaddress, pyping, pysnmp, 
* https://netaddr.readthedoc.io/
* https://docs.python.org/dev/library/ipaddress.html


## RUBY (Useful for Chef)
* http://www.ruby-lang.org/en/
* http://ruby-doc.org/
* https://en.wikipedia.org/wiki/Why%27s_(poignant)_Guide_to_Ruby


## Open-source Configuration Management Software
* https://en.wikipedia.org/wiki/Comparison_of_open-source_configuration_management_software
  
Good podcasts on these topics on Packet Pushers 
* Show 176: Intro To Python & Automation For Network Engineers 
  http://packetpushers.net/podcast/podcasts/show-176-intro-to-python-automation-for-network-engineers
* Show 198: Kirk Byers On Network Automation With Python & Ansible  
  http://packetpushers.net/podcast/podcasts/show-198-kirk-byers-network-automation-python-ansible
* Show 270: Design & Build 9: Automation With Python And Netmiko 
  http://packetpushers.net/podcast/podcasts/show-270-design-build-9-automation-python-netmiko
* Datanauts 034: Automate All The Packets
  http://packetpushers.net/podcast/podcasts/datanauts-034-automate-packets
* PQ Show 81: Network Testing With ToDD
  http://packetpushers.net/podcast/podcasts/pq-show-81-network-testing-todd
* PQ Show 99: Netmiko & NAPALM For Network Automation 
  http://packetpushers.net/podcast/podcasts/pq-show-99-netmiko-napalm-network-automation


Chef & Puppet are the older tools 

## CHEF
Chef is a configuration management tool written in Ruby, and uses a pure Ruby DSL for writing configuration "recipes". These recipes contain resources that should be put into the declared state. Chef can be used as a client–server tool, or used in "solo" mode
* https://www.chef.io/
* https://learn.chef.io/
* https://github.com/chef/chef
    
## PUPPET
Puppet consists of a custom declarative language to describe system configuration, distributed using the client–server paradigm, and a library to realize the configuration. The resource abstraction layer enables administrators to describe the configuration in high-level terms, such as users, services and packages. Puppet will then ensure the server's state matches the description. 
* https://puppet.com/
* https://puppet.com/resources/ebook/tools-for-learning-puppet
* https://github.com/puppetlabs
LEARNING LAB: 
* https://puppet.com/download-learning-vm  


One engineers view of Salt & Ansible, useful for an overview of both:
* http://jensrantil.github.io/salt-vs-ansible.html

## ANSIBLE
Combines multi-node deployment, ad-hoc task execution, and configuration management in one package. Manages nodes over SSH and requires python (2.4 or later) to be installed on them. Modules work over JSON and standard output and can be written in any language. Uses YAML to express reusable descriptions of systems.
* https://www.ansible.com/
* https://www.ansible.com/quick-start-video
* https://www.ansible.com/network-automation
* http://docs.ansible.com/ansible/index.html
* https://github.com/ansible/ansible
* https://networklore.com/ansible-getting-started/
* http://jpmens.net/2012/06/06/configuration-management-with-ansible/
* https://galaxy.ansible.com/Juniper/junos/
* http://docs.ansible.com/ansible/intro_networking.html
* http://docs.ansible.com/ansible/ios_config_module.html
LEARNING LAB:
* https://www.turnkeylinux.org/ansible **Ansible on a VM**
* https://github.com/turnkeylinux-apps/ansible/blob/master/docs/usage.rst

## SALT
Salt started out as a tool for remote server management. As its usage has grown, it has gained a number of extended features, including a more comprehensive mechanism for host configuration. This is a relatively new feature facilitated through the Salt States component. With the traction that Salt has gotten in the last bit, the support for more features and platforms might continue to grow.
* https://saltstack.com/community/ <-best starting point
* https://blog.talpor.com/2014/07/saltstack-beginners-tutorial/
LEARNING LAB: **uses Vagrant on Virtual Box to setup the lab ie automation in action**
* https://docs.saltstack.com/en/getstarted/fundamentals/index.html 

Been around for awhile:

## RANCID
RANCID monitors a router's (or more generally a device's) configuration, including software and hardware (cards, serial numbers, etc) and uses CVS (Concurrent Version System) or Subversion to maintain history of changes
* http://www.shrubbery.net/rancid/

## OXIDIZED:
Oxidized is a network device configuration backup tool. It's a RANCID replacement!
* https://github.com/ytti/oxidized


## VAGRANT
Vagrant is computer software that creates and configures virtual development environments. It can be seen as a higher-level wrapper around virtualization software such as VirtualBox, VMware, KVM and Linux Containers (LXC), and around configuration management software such as Ansible, Chef, Salt, and Puppet.
* https://www.vagrantup.com/
* http://www.vagrantbox.es/
* http://www.cyberciti.biz/cloud-computing/use-vagrant-to-create-small-virtual-lab-on-linux-osx/

## VirtualBox
Free equiv to VMware Workstation Pro and you can create desktop shortcuts to start VMs directly
* https://www.virtualbox.org/wiki/Downloads
* https://www.virtualbox.org/manual/ch06.html
How to hook your VMware Workstation VM and Virtual Box VM together (to manage VIRL devices etc)
* http://www.sysprobs.com/setup-network-virtualbox-vmware-virtual-machines

## VMware stuff:
* https://rednectar.net/2011/07/20/vmware-interfaces-tutorial/
* http://www.virtualizationadmin.com/articles-tutorials/vmware-server-workstation-player-articles/understanding-virtual-networking-vmware-workstation-9.html
     
## Turnkey Linux 
VMs/ISOs/containers for various purposes:
* https://www.turnkeylinux.org/
* https://www.turnkeylinux.org/core  
* https://www.turnkeylinux.org/ansible

## YAML: YAML Ain't Markup Language
YAML is a human friendly data serialization standard for all programming languages.
* http://yaml.org/
* http://docs.ansible.com/ansible/YAMLSyntax.html
* http://www.yaml.org/spec/1.2/spec.html

## JSON 
(JavaScript Object Notation) is a lightweight data-interchange format. Seems to be used a lot by newer automation approaches
* http://json.org/

## Utilities

DNS (The virtual world)
* https://www.turnkeylinux.org/forum/general/20110413/simplest-dns-server
* http://www.virtualizationhowto.com/2015/04/lightweight-dns-server-vmware-lab/

IP address management (IPAM) and data center infrastructure management (DCIM) tool. 
* https://github.com/digitalocean/netbox


## Front ends 
(really more like 'getting severely sidetracked')    
*  https://www.airpair.com/python/posts/django-flask-pyramid

###     DJANGO
Django is a high-level Python Web framework that encourages rapid development and clean, pragmatic design. 
* https://www.djangoproject.com/
* https://docs.djangoproject.com/en/1.9/intro/tutorial01/
* https://www.turnkeylinux.org/django

###     Pyramid
similar purpose to Django
* http://www.pylonsproject.org/

###     Flask
similar purpose to Django but simpler
* http://flask.pocoo.org/
* https://pypi.python.org/pypi/Flask/0.11
