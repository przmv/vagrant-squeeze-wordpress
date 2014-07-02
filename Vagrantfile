# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "puppetlabs/debian-6.0.9-64-nocm"
  config.vm.hostname = "squeeze-wordpress"
  config.ssh.forward_agent = true
  config.vm.network :private_network, ip: "192.168.50.4"
  config.vm.provision :ansible, :playbook => "site.yml"
end
