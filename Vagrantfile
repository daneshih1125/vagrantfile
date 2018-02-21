# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"

  config.vm.define "xenial01" do |xenial01|
    xenial01.vm.box = "ubuntu/xenial64"
    xenial01.vm.hostname = 'xenial01'
    xenial01.vm.box_url = "ubuntu/xenial64"
    xenial01.vm.network :private_network, ip: "192.168.67.11"
    xenial01.vm.provider :virtualbox do |v|
      v.customize ["modifyvm", :id, "--memory", 2048]
    end
  end
end
