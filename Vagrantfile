# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.network "private_network", ip: "192.168.33.10"

  config.vm.provision "shell", inline: <<-SHELL
    sudo apt-get update
    sudo apt-get install -y apache2
  SHELL

  config.vm.synced_folder "./public_html/", "/var/www/html", :mount_options => ["dmode=777", "fmode=666"]

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "1024"
  end

end
