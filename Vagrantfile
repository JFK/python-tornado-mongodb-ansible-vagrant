# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.ssh.insert_key = false
  config.vm.define "site" do |site|
    site.vm.box = "ARTACK/debian-jessie"
    site.vm.box_url = "https://atlas.hashicorp.com/ARTACK/boxes/debian-jessie"
    site.vm.network :private_network, ip: "192.168.33.100"

    site.vm.provision "ansible" do |ansible| 
      ansible.playbook = "site.yml"
      ansible.verbose = 'vvv'
    end 
  end

end
