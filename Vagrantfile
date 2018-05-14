# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/trusty64"

    # set the hostname
    config.vm.hostname = "evhive.dev"

    #set the shared folder
    config.vm.synced_folder "src", "/home/vagrant/workspace/src"

    #provision the box
    config.vm.provision :shell, :path => "setup/install.sh"

end