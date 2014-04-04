# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "centos6"
  config.vm.provider 'virtualbox' do |v|
    v.memory = 1024
  end

  config.vm.provision 'shell', inline: 'sudo yum install puppet -y'

  config.vm.provision :puppet
end
