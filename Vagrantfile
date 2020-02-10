Vagrant.configure("2") do |config|
  config.vm.box = "generic/centos8"
  
  config.vm.provision "shell", inline: <<-SHELL
    echo "Installing bpftrace and bcc"
    dnf -yq install bpftrace bcc 
  SHELL

  config.vm.synced_folder "samples/", "/tmp/samples"
end
