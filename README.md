# Vagrant Box for MongoDB Training

Contains:

 * Ubuntu 16.04
 * Node.js
 * MongoDB 3.6
 * mtools
 * Express

Port 3000 is configured to forward to host computer.  Additional ports can be configured in the `Vagrantfile`

## Prerequisites

 * Vagrant
 * VirtualBox

### Starting

What things you need to install the software and how to install them

```
git clone git@github.com:jaydestro/mdb-vagrant.git
cd mdb-vagrant
vagrant up
```

Once completed with the installation you will be able to `vagrant ssh` to log into the provisioned Ubuntu Server.
