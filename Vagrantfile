# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define "devbox" do |devbox|
    devbox.vm.box = "ubuntu/bionic64"
    devbox.vm.provision "shell", path: "scripts/install.sh"
    devbox.vm.provider "virtualbox" do |v|
      v.memory = 4096
      v.cpus = 2
    end
  end
end
