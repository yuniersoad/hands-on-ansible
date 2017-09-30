# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|

# Not really required, local computer can be used instead
#  config.vm.define "acs" do |acs|
#    acs.vm.box = "ubuntu/trusty64"
#    acs.vm.hostname = "acs"
#    acs.vm.network "private_network", ip: "192.168.33.10"
#  end

  config.vm.define "web" do |web|
    web.vm.box = "ubuntu/trusty64"
    web.vm.hostname = "web"
    web.vm.network "private_network", ip: "192.168.33.20"
    web.vm.network "forwarded_port", guest: 80, host:8080
  end

  config.vm.define "db" do |db|
    db.vm.box = "ubuntu/trusty64"
    db.vm.hostname = "db"
    db.vm.network "private_network", ip: "192.168.33.30"
  end
end
