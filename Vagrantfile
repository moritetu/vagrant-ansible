Vagrant.configure(2) do |config|
  config.vm.box = "centos/7"
  config.vm.network "forwarded_port", guest: 22, host: 2225
  config.vm.provision "ansible" do |ansible|
    ansible.verbose  = true
    ansible.playbook = "vagrant.yml"
  end
end
