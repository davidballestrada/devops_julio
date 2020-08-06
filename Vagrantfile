# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.ssh.insert_key = false
  config.vm.define "base2" do | maquina1 |
    maquina1.vm.box = "gold"
    maquina1.ssh.insert_key = false
    # maquina1.vm.network "private_network", ip: "190.100.100.190"
    maquina1.vm.network "private_network", ip: "192.168.100.190"

    # maquina1.vm.synced_folder "./www", "/vagrant_data"
    maquina1.vm.hostname = "gold"
    maquina1.vm.provider "virtualbox" do | vb |
      vb.memory = "4096"
      vb.cpus = 4
      vb.name = "gold2"
      maquina1.vm.disk :disk, size: "20GB", name: "scsi_001"
   end
  end
   config.vm.define "base3" do | maquina1 |
    maquina1.vm.box = "gold"
    maquina1.ssh.insert_key = false
    # maquina1.vm.network "private_network", ip: "190.100.100.190"
    maquina1.vm.network "private_network", ip: "192.168.100.191"

    # maquina1.vm.synced_folder "./www", "/vagrant_data"
    maquina1.vm.hostname = "gold1"
    maquina1.vm.provider "virtualbox" do | vb |
      vb.memory = "4096"
      vb.cpus = 4
      vb.name = "gold3"
      maquina1.vm.disk :disk, size: "20GB", name: "scsi_001"
   end
  end
   
    # maquina1.vm.disk : disk, size: "10GB", primary:true
    

    # (1..2).each do | x |
    #   config.vm.define "test#{x}" do | maquina1 | 
    #     maquina1.vm.box = "machineServer"
    #     maquina1.ssh.insert_key = false
    #     maquina1.vm.network "private_network", ip: "190.100.100.19#{x}"
    #     maquina1.vm.synced_folder "./www", "/vagrant_data"
    #     maquina1.vm.hostname = "webserver#{x}"
    #     maquina1.vm.provider "virtualbox" do | vb |
    #       vb.memory = "4096"
    #       vb.cpus = 4
    #       vb.name = "machines#{x}"
    #       #maquina1.vm.disk :disk, size: "10GB", name: "scsi_001"
    #     end
    #     maquina1.vm.provision "shell", inline: <<-SHELL
    #       sudo yum install -y httpd
    #     SHELL
    #   end
    # end 

end
