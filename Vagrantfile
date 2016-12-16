# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "sonico999/devcode"

  config.ssh.username = 'vagrant'
  config.ssh.password = 'vagrant'
  # ip privado
  config.vm.network "private_network", ip: "192.168.33.10"
  
  # ip publico
  config.vm.network "public_network", ip: "192.168.1.241"
  
  # puerto de mysql
  config.vm.network "forwarded_port", guest: 3306, host: 33060
  
  # ngnix
  config.vm.network :forwarded_port, guest: 80, host: 8000, auto_correct: true
  
  # configurar carpeta a compartir ("/Users/eveR/WebProjects")
  config.vm.synced_folder "/Users/eveR/WebProjects", "/home/vagrant/Code", create: true, group: "vagrant", owner: "vagrant"

  config.vm.provider "virtualbox" do |vb|
  # ram
     vb.memory = "2048"
  end
  
end
