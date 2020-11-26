Vagrant.configure("2") do |config|
  config.vm.define "crc", primary: true do |crc|
    crc.vm.box = "ubuntu/bionic64"
    crc.vm.network "forwarded_port", guest: 22, host: 2222
    crc.vm.provider "virtualbox" do |vb|
      vb.memory = "10240"
    end
  end


  #
  # View the documentation for the provider you are using for more
  # information on available options.

  # Enable provisioning with a shell script. Additional provisioners such as
  # Ansible, Chef, Docker, Puppet and Salt are also available. Please see the
  # documentation for more information about their specific syntax and use.
  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   apt-get install -y apache2
  # SHELL
end
