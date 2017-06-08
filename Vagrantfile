# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure("2") do |config|
 
  config.vm.box = "chad-thompson-VAGRANTSLASH-ubuntu-trusty64-gui"
  config.vm.synced_folder "../shared", "/opt/shared"

   
   config.vm.provider "virtualbox" do |vb|	
	 #vb.gui = true
     vb.memory = "2096"
	 vb.cpus = "2"
   end
  
  
  config.vm.define "AnsiMasterEZ" do |masterNode|
	masterNode.vm.hostname = "AnsiMasterEZ1"
	masterNode.vm.network "public_network", ip: "192.168.1.106"
	#config.vm.provision "shell", path: "bootstrap3.sh"
  end
  
   config.vm.define "AnsiSlaveEZ" do |slaveNode|
	slaveNode.vm.hostname = "AnsiSlaveEZ1"
	slaveNode.vm.network "public_network", ip: "192.168.1.105"
	#config.vm.provision "shell", path: "bootstrap3.sh"
  end
  
	
	
end
