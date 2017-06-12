# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.

Vagrant.configure("2") do |config|

  config.vm.define "ansiblemaster" do |ansiblemaster|
    ansiblemaster.vm.box = "centos/7"
    ansiblemaster.vm.hostname = 'ansiblemaster'
    ansiblemaster.vbguest.auto_update = true
    ansiblemaster.vm.synced_folder "shared/", "/tmp/shared"
    
    ansiblemaster.vm.network :private_network, ip: "192.168.30.105"
      
    ansiblemaster.vm.provider :virtualbox do |vb|
      vb.gui = false
      vb.linked_clone = true
      vb.memory = 4096
      vb.cpus = 2
      vb.customize ["modifyvm", :id, "--name", "ansiblemaster"]
    end
    ansiblemaster.vm.provision "shell", inline: $install_ansible
  end

  config.vm.define "splunkidx01" do |splunkidx01|
    splunkidx01.vm.box = "centos/7"
    splunkidx01.vm.hostname = 'splunkidx01'
    splunkidx01.vbguest.auto_update = true
    splunkidx01.vm.synced_folder "shared/", "/tmp/shared"

    splunkidx01.vm.network :private_network, ip: "192.168.30.106"
      
    splunkidx01.vm.provider :virtualbox do |vb|
      vb.gui = false
      vb.linked_clone = true
      vb.memory = 4096
      vb.cpus = 4
      vb.customize ["modifyvm", :id, "--name", "splunkidx01"]
    end
    splunkidx01.vm.provision "shell", inline: $authorized_keys
  end

  config.vm.define "splunkidx02" do |splunkidx02|
    splunkidx02.vm.box = "centos/7"
    splunkidx02.vm.hostname = 'splunkidx02'
    splunkidx02.vbguest.auto_update = true
    splunkidx02.vm.synced_folder "shared/", "/tmp/shared"

    splunkidx02.vm.network :private_network, ip: "192.168.30.107"
      
    splunkidx02.vm.provider :virtualbox do |vb|
      vb.gui = false
      vb.linked_clone = true
      vb.memory = 4096
      vb.cpus = 4
      vb.customize ["modifyvm", :id, "--name", "splunkidx02"]
    end
    splunkidx02.vm.provision "shell", inline: $authorized_keys
  end

  config.vm.define "splunkidx03" do |splunkidx03|
    splunkidx03.vm.box = "centos/7"
    splunkidx03.vm.hostname = 'splunkidx03'
    splunkidx03.vbguest.auto_update = true
    splunkidx03.vm.synced_folder "shared/", "/tmp/shared"

    splunkidx03.vm.network :private_network, ip: "192.168.30.108"
      
    splunkidx03.vm.provider :virtualbox do |vb|
      vb.gui = false
      vb.linked_clone = true
      vb.memory = 4096
      vb.cpus = 4
      vb.customize ["modifyvm", :id, "--name", "splunkidx03"]
    end
    splunkidx03.vm.provision "shell", inline: $authorized_keys
  end

config.vm.define "splunkshc01" do |splunkshc01|
    splunkshc01.vm.box = "centos/7"
    splunkshc01.vm.hostname = 'splunkshc01'
    splunkshc01.vbguest.auto_update = true
    splunkshc01.vm.synced_folder "shared/", "/tmp/shared"

    splunkshc01.vm.network :private_network, ip: "192.168.30.109"
      
    splunkshc01.vm.provider :virtualbox do |vb|
      vb.gui = false
      vb.linked_clone = true
      vb.memory = 4096
      vb.cpus = 4
      vb.customize ["modifyvm", :id, "--name", "splunkshc01"]
    end
    splunkshc01.vm.provision "shell", inline: $authorized_keys
  end  

config.vm.define "splunkshc02" do |splunkshc02|
    splunkshc02.vm.box = "centos/7"
    splunkshc02.vm.hostname = 'splunkshc02'
    splunkshc02.vbguest.auto_update = true
    splunkshc02.vm.synced_folder "shared/", "/tmp/shared"

    splunkshc02.vm.network :private_network, ip: "192.168.30.110"
      
    splunkshc02.vm.provider :virtualbox do |vb|
      vb.gui = false
      vb.linked_clone = true
      vb.memory = 4096
      vb.cpus = 4
      vb.customize ["modifyvm", :id, "--name", "splunkshc02"]
    end
    splunkshc02.vm.provision "shell", inline: $authorized_keys
  end

config.vm.define "splunkshc03" do |splunkshc03|
    splunkshc03.vm.box = "centos/7"
    splunkshc03.vm.hostname = 'splunkshc03'
    splunkshc03.vbguest.auto_update = true
    splunkshc03.vm.synced_folder "shared/", "/tmp/shared"

    splunkshc03.vm.network :private_network, ip: "192.168.30.111"
      
    splunkshc03.vm.provider :virtualbox do |vb|
      vb.gui = false
      vb.linked_clone = true
      vb.memory = 4096
      vb.cpus = 4
      vb.customize ["modifyvm", :id, "--name", "splunkshc03"]
    end
    splunkshc03.vm.provision "shell", inline: $authorized_keys
  end

config.vm.define "splunkcm01" do |splunkcm01|
    splunkcm01.vm.box = "centos/7"
    splunkcm01.vm.hostname = 'splunkcm01'
    splunkcm01.vbguest.auto_update = true
    splunkcm01.vm.synced_folder "shared/", "/tmp/shared"

    splunkcm01.vm.network :private_network, ip: "192.168.30.112"
      
    splunkcm01.vm.provider :virtualbox do |vb|
      vb.gui = false
      vb.linked_clone = true
      vb.memory = 4096
      vb.cpus = 4
      vb.customize ["modifyvm", :id, "--name", "splunkcm01"]
    end
    splunkcm01.vm.provision "shell", inline: $authorized_keys
  end

config.vm.define "splunkuf01" do |splunkuf01|
    splunkuf01.vm.box = "centos/7"
    splunkuf01.vm.hostname = 'splunkuf01'
    splunkuf01.vbguest.auto_update = true
    splunkuf01.vm.synced_folder "shared/", "/tmp/shared"

    splunkuf01.vm.network :private_network, ip: "192.168.30.113"
      
    splunkuf01.vm.provider :virtualbox do |vb|
      vb.gui = false
      vb.linked_clone = true
      vb.memory = 4096
      vb.cpus = 2
      vb.customize ["modifyvm", :id, "--name", "splunkuf01"]
    end
    splunkuf01.vm.provision "shell", inline: $authorized_keys
  end

config.vm.define "splunkuf02" do |splunkuf02|
    splunkuf02.vm.box = "centos/7"
    splunkuf02.vm.hostname = 'splunkuf02'
    splunkuf02.vbguest.auto_update = true
    splunkuf02.vm.synced_folder "shared/", "/tmp/shared"

    splunkuf02.vm.network :private_network, ip: "192.168.30.114"
      
    splunkuf02.vm.provider :virtualbox do |vb|
      vb.gui = false
      vb.linked_clone = true
      vb.memory = 4096
      vb.cpus = 2
      vb.customize ["modifyvm", :id, "--name", "splunkuf02"]
    end
    splunkuf02.vm.provision "shell", inline: $authorized_keys
  end

$authorized_keys = <<SCRIPT
echo Adding ansiblemaster SSH pub key...
sudo -u vagrant cat /tmp/shared/ansiblemaster.pub >> /home/vagrant/.ssh/authorized_keys
sudo -u vagrant sort /home/vagrant/.ssh/authorized_keys | uniq > /home/vagrant/.ssh/authorized_keys.uniq
sudo -u vagrant mv -f /home/vagrant/.ssh/authorized_keys{.uniq,}
sudo cp /tmp/shared/hosts.etc /etc/hosts
echo Done installing SSH keys!
SCRIPT

$install_ansible = <<SCRIPT
echo Installing Ansible...
sudo yum -y install epel-release ; sudo yum -y install git python python-devel python-pip openssl ansible
sudo cp /tmp/shared/hosts.etc /etc/hosts
sudo cp /tmp/shared/hosts.ansible /etc/ansible/hosts
sudo sed -i '/host_key_checking = False/s/^#//g' /etc/ansible/ansible.cfg
sudo sed -i '/GSSAPIAuthentication yes/s/yes/no/g' /etc/ssh/sshd_config
if sudo -u vagrant [ ! -f /home/vagrant/.ssh/id_rsa ]; then 
  sudo -u vagrant ssh-keygen -q -f /home/vagrant/.ssh/id_rsa -N ""
  sudo -u vagrant cp /home/vagrant/.ssh/id_rsa.pub /tmp/shared/$HOSTNAME.pub
  sudo -u vagrant cat /tmp/shared/ansiblemaster.pub >> /home/vagrant/.ssh/authorized_keys
  sudo -u vagrant sort /home/vagrant/.ssh/authorized_keys | uniq > /home/vagrant/.ssh/authorized_keys.uniq
  sudo -u vagrant mv -f /home/vagrant/.ssh/authorized_keys{.uniq,}
fi  
echo Done installing Ansible!
SCRIPT

end
