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

    #port forwarding
    config.vm.network "forwarded_port", guest: 8085, host: 8085,
        auto_correct: true

end