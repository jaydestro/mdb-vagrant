Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.box_check_update = false
  config.vm.hostname = "community.mongodb.com"
  config.vm.network "forwarded_port", guest: 3000, host:3000 
  config.vm.network :private_network, ip: "192.168.14.100"
  config.vm.provision :shell, path: "provision-mongod", args: ENV['ARGS']

  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--cpus", "1", "--memory", 1024]
  end

  config.vm.synced_folder "shared/", "/shared", create: true
end
