# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://atlas.hashicorp.com/search.
#  config.vm.box = "mauricepacker"
  config.vm.box = "Centos1"
  config.vm.provider "virtualbox" do |v|
    v.gui = false
    config.ssh.pty = true
end

config.vm.define "app2" do | app_config |
 app_config.vm.host_name = "app2"
 app_config.vm.network :private_network, ip: "192.168.56.36" 
# app_config.vm.provision :ansible do |ansible|
#        ansible.inventory_path = "/Users/mauricesheehan/Testing"
#	ansible.playbook = "common.yaml"
# end
end
end
