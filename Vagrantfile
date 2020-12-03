# -*- mode: ruby -*-
# vi: set ft=ruby :

ENV['VAGRANT_DEFAULT_PROVIDER'] = 'virtualbox'

Vagrant.configure("2") do |config|
  ##### DEFINE VM #####
  config.vm.define "ubuntu-01" do |config|
  config.vm.hostname = "ubuntu-01"
  config.vm.box = "ubuntu/bionic64"
  config.vm.box_check_update = false
  #config.vm.forwarded_port 80, 8080
  config.vm.network "public_network", bridge:"Intel(R) Dual Band Wireless-AC 8265"
  end
end