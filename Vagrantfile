Vagrant::Config.run do |config|
  config.vm.box = "ubuntu-12.04-amd64"

  # THE URL FROM WHERE THE 'CONFIG.VM.BOX' BOX WILL BE FETCHED IF IT
  # DOESN'T ALREADY EXIST ON THE USER'S SYSTEM.
  config.vm.box_url = "http://dl.dropbox.com/u/4031118/Vagrant/ubuntu-12.04.1-server-i686-virtual.box"
  config.vm.forward_port 6379, 6379
  config.vm.customize ["modifyvm", :id, "--memory", 1024]

  config.vm.provision :shell, :path => "init.sh"
end
