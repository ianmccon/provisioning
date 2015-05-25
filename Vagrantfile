# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
    config.vm.box = "precise32"
    config.vm.box_url = "http://files.vagrantup.com/precise32.box"

    config.vm.network :private_network, ip: "10.10.10.10"

    config.vm.provision "ansible" do |ansible|
        ansible.playbook = "provision.yml"
    end
end
