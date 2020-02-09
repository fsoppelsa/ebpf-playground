Vagrant.configure("2") do |config|
  config.vm.box = "generic/centos8"

  config.vm.provision "shell", inline: <<-SHELL
    dnf -y install bpftrace bcc
  SHELL
end
