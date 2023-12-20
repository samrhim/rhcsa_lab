# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "generic/centos9s"
    config.vm.define "server" do |server|
      server.vm.hostname = "server"
      server.vm.network "private_network", ip: "192.168.56.10"
      server.vm.provider "virtualbox" do |vb|
        vb.memory = "4096"
        vb.cpus = 2
		vb.name = "server"
      end
    end
    config.vm.define "client" do |client|
      client.vm.hostname = "client"
      client.vm.network "private_network", ip: "192.168.56.11"
      client.vm.provider "virtualbox" do |vb|
        vb.memory = "2048"
        vb.cpus = 2
		vb.name = "client"
      end
    end
end