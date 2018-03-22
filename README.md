# Vagrant Box for MongoDB Training

Contains:

 * [Ubuntu 16.04 LTS](https://www.ubuntu.com/download)
 * [Node.js](https://nodejs.org/en/)
 * [MongoDB 3.6](https://www.mongodb.com/mongodb-3.6)
 * [mtools](https://github.com/rueckstiess/mtools)
 * [Express](https://expressjs.com)
 * [Scotch.io "Node-Todo"](https://github.com/scotch-io/node-todo)

Port 3000 and 8080 are configured to forward to host computer.  Additional ports can be configured in the `Vagrantfile`

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

### Scotch.io "Node-Todo"

This simple ["todo"](https://github.com/scotch-io/node-todo) single page application has been cloned from git and allows you to begin learning ho to launch and modify as simple Node.js application.

To begin working with this application, enter the `/home/vagrant/node-todo` directory.  There you can review the connection string in `config/database.js` for your database connection to MongoDB.  You can modify this connection to have this data read and written from a local MongoDB database installation or from a remote connection, such as [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).

(https://imgur.com/a/Hc1tt)


### Local access

If you're working on a Node.js app with the port 3000 or 8080, you'll be able to access the app via http://localhost:3000 or http://localhost:8080.  
