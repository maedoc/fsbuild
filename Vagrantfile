# -*- mode: ruby -*-
# vi: set ft=ruby sw=2 sts=2 et ai :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.ssh.forward_agent = true
  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 4
  end
  config.vm.provision "ansible_local" do |ansible| ansible.playbook = "playbook.yml" end
end
