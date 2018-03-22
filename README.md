# Vagrant Box for MongoDB Training

Contains:

 * [Ubuntu] 16.04(https://www.ubuntu.com/download)
 * [Node.js](https://nodejs.org/en/)
 * [MongoDB 3.6](https://www.mongodb.com/mongodb-3.6)
 * [mtools](https://github.com/rueckstiess/mtools)
 * [Express](https://expressjs.com)

Port 3000 is configured to forward to host computer.  Additional ports can be configured in the `Vagrantfile`

## Prerequisites

 * [Vagrant](http://vagrantup.com/)
 * [VirtualBox](https://www.virtualbox.org/)

 These are both available for all major platforms. (Windows, OS X, Linux)

### Starting

Download the box by cloning, cd into directory and then `vagrant up` the box.  

```
git clone git@github.com:jaydestro/mdb-vagrant.git
cd mdb-vagrant
vagrant up
```

Once completed with the installation you will be able to `vagrant ssh` to log into the provisioned Ubuntu Server.


### Terminate

First, `exit` from the shell you entered with `vagrant ssh` and then when returned to the host system:

```
vagrant destroy
```

### Local access

If you're working on a Node.js app with the port 3000, you'll be able to access the app via http://localhost:3000.  
