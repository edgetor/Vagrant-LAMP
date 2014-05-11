# Vagrant LAMP Files
Copy `Vagrantfile` and `Berksfile` into directory.

## Description
A Vagrant script designed for a basic LAMP setup.

`Chef` is used for provisioning and `Berkshelf` is used to manage cookbooks.

--- 
## Requirements
* [VirtualBox](https://www.virtualbox.org)
* [Vagrant](http://vagrantup.com)
* [Berkshelf](http://berkshelf.com)
	* `gem install berkshelf`
* [vagrant-berkshelf](https://github.com/riotgames/vagrant-berkshelf)
	* `vagrant plugin install vagrant-berkshelf`
* [vagrant-hostmanager](https://github.com/smdahlen/vagrant-hostmanager)
	* `vagrant plugin install vagrant-hostmanager`

---
## Installation
* `$ cd projectname`
* `$ curl -O https://raw.githubusercontent.com/edgetor/Vagrant-LAMP/master/\{Vagrantfile,Berksfile\}`
* Edit Vagrantfile
  * Set Host-only network IP (ip\_address)
  * Set Project Name IP (project\_name)
  * Set Root Database password (database\_password)
* `$ vagrant up`

Host file modified to point project at [http://projectname.local](http://projectname.local)

---
## Installed software
* Ubuntu Trusty
* Apache **2.4**
* MySQL
* PHP **5.5** (with apcu, mysql, curl, mcrypt, memcached, gd)
* phpMyAdmin
* memcached
* Postfix
* XDebug
* Grunt
* composer
* curl
* vim, git, screen, zsh
* phpunit

---
## Default credentials
### MySQL
* Username: root
* Password: mysecretpassword
* Port: 3306

### PostgreSQL
* Username: root
* Password: mysecretpassword
* Port: 5432

### Memcached
* Port: 11211
