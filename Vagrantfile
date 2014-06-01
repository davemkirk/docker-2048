# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

## Set the default provider to docker.
#ENV['VAGRANT_DEFAULT_PROVIDER'] = "docker"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

    config.vm.define "2048" do |v|
        v.vm.provider "docker" do |d|
            d.vagrant_vagrantfile = "Dockerhost"
            d.build_dir = "."
            d.ports = ["8080:80"]

        end
    end

end
