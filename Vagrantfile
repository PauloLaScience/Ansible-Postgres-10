# -*- mode: ruby -*-
# vi: set ft=ruby :
# Vagrantfile
Vagrant.configure(2) do |config|
    config.vm.box = 'centos/7'
    config.vm.provider 'libvirt' do |lv|
        lv.cpus = 1
        lv.memory = 1024
    end
    config.vm.provision "ansible" do |ansible|
        ansible.playbook = "installpg10.yml"
    end
end
