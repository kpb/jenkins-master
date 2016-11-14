# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "bento/ubuntu-16.04"

  # Forward 8080 to the host
  config.vm.network "forwarded_port", guest: 8080, host: 8080

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
    vb.name = "jenkins-master"
  end

  # provision with ansible_local
  config.vm.provision :ansible_local do |ansible|
    ansible.sudo = true
    # true to debug
    ansible.verbose = true
    ansible.playbook = "provisioning/jenkins-master.yml"
  end
  
end
