# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant::Config.run do |config|
  # Set box configuration
  config.vm.box = "lucid32"
  #config.vm.box_url = "http://files.vagrantup.com/lucid32.box"

  # Assign this VM to a host-only network IP, allowing you to access it via the IP.
  config.vm.network :hostonly, "192.168.10.50"

  # Enable provisioning with chef solo, specifying a cookbooks path (relative
  # to this Vagrantfile), and adding some recipes and/or roles.
  #
  config.vm.provision :chef_solo do |chef|
    chef.cookbooks_path = "cookbooks"
    chef.add_recipe "vagrant_main"
  end
end
