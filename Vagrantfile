Vagrant.configure(2) do |config|
  config.vm.box = "precise32"

  config.vm.network "private_network", ip: "192.168.0.99"

  config.vm.provision :ansible do |ansible|
    ansible.playbook = "provision.yml"
  end
end
