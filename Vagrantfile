Vagrant.configure("2") do |config|
  config.vm.box = "debian/bullseye64"
  config.vm.hostname = "asnible"
  config.vm.network "public_network"
  config.vm.synced_folder "./ansible", "/ansible"
  config.vm.provider "virtualbox" do |vb|
    vb.name = "Zabbix-Ansible"
    vb.memory = "2048"
    vb.cpus = 2
  end
  config.vm.provision "shell", inline: <<-SHELL
    apt update
    apt install ansible -y
    ansible-playbook --connection=local /ansible/playbook.yml
  SHELL
end
