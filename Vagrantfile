Vagrant.configure("2") do |config|
  config.vm.define "swarm_manager", primary: true do |host|
    host.vm.box = "ubuntu/bionic64"
    host.vm.network "forwarded_port", guest: 22, host: 2222, auto_correct: true
    host.vm.network "forwarded_port", guest: 2377, host: 2377, auto_correct: true
    host.vm.network "forwarded_port", guest: 7946, host: 7946, auto_correct: true
    host.vm.network "forwarded_port", guest: 4789, host: 4789, protocol: :udp, auto_correct: true

    # crc.vm.provider "virtualbox" do |vb|
    #   vb.memory = "1024"
    # end
    # config.vm.provision "shell", inline: <<-SHELL
    #   apt-get update
    #   apt-get install -y apache2
    # SHELL
  end

  config.vm.define "swarm_worker_1", primary: true do |host|
    host.vm.box = "ubuntu/bionic64"
    host.vm.network "forwarded_port", guest: 22, host: 2222, auto_correct: true
    host.vm.network "forwarded_port", guest: 2377, host: 2377, auto_correct: true
    host.vm.network "forwarded_port", guest: 7946, host: 7946, auto_correct: true
    host.vm.network "forwarded_port", guest: 4789, host: 4789, protocol: :udp, auto_correct: true
    
    # crc.vm.provider "virtualbox" do |vb|
    #   vb.memory = "1024"
    # end
    # config.vm.provision "shell", inline: <<-SHELL
    #   apt-get update
    #   apt-get install -y apache2
    # SHELL
  end
  config.vm.define "swarm_worker_2", primary: true do |host|
    host.vm.box = "ubuntu/bionic64"
    host.vm.network "forwarded_port", guest: 22, host: 2222, auto_correct: true
    host.vm.network "forwarded_port", guest: 2377, host: 2377, auto_correct: true
    host.vm.network "forwarded_port", guest: 7946, host: 7946, auto_correct: true
    host.vm.network "forwarded_port", guest: 4789, host: 4789, protocol: :udp, auto_correct: true
    
    # crc.vm.provider "virtualbox" do |vb|
    #   vb.memory = "1024"
    # end
    # config.vm.provision "shell", inline: <<-SHELL
    #   apt-get update
    #   apt-get install -y apache2
    # SHELL
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
