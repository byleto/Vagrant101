Vagrant.configure(2) do |config|
config.vm.box = "milmih/precise32-ruby"
config.vm.network "forwarded_port", guest: 80, host: 8080
config.vm.provider "virtualbox" do |vb|
  # Display the VirtualBox GUI when booting the machine
  vb.gui = true
   
  # Customize the amount of memory on the VM:
  vb.memory = "1024"
  end
  # Enable provisioning with a shell script.
  config.vm.provision "shell", inline: "sudo apt-get install -y apache2"
  
end