
Vagrant.configure(2) do |config|
  # base image
  config.vm.box = "ubuntu/ubuntu-core-devel-amd64"

  config.vm.hostname = "node-dev-env"

  config.vm.synced_folder "work_space/",  "/home/vagrant/work_space"

  config.vm.provision "shell",  :path => "provision.sh"

  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm",  :id,  "--memory",  "1024"]
  end

end
