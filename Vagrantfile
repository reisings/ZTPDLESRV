# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "sreisinger/centos7ztp"
  config.vm.box_version = "0.0.1"
  config.vm.provider "virtualbox"
  config.ssh.port = 22
  config.ssh.username = 'vagrant'
  config.ssh.host = '192.168.56.20'
  config.ssh.password = 'Juniper123'

  # Management ports
  config.vm.network 'public_network', ip: "192.168.2.192", nic_type: '82540EM', virtualbox__bridged: "BRIDGED_EXTERNAL"
  config.vm.network 'private_network', ip: "10.1.1.1", nic_type: 'virtio', virtualbox__intnet: "ZTP_Internal"
  config.vm.network 'private_network', ip: "192.168.56.20", nic_type: '82540EM', virtualbox__hostonly: "HOST"

  #FIX NAT INTERFACE NOT ACTIVATED
  config.vm.provider 'virtualbox' do |vb|
    vb.customize ['modifyvm', :id, '--cableconnected1', 'on']
  end
  
end

