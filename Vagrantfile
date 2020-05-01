Vagrant.configure(2) do |config|
	config.vm.define "devops-box" do |devbox|
		devbox.vm.box = "hashicorp/bionic64"
    		#devbox.vm.network "private_network", ip: "192.168.199.9"
    		#devbox.vm.hostname = "devops-box"
      		devbox.vm.provision "shell", path: "scripts/install.sh"
    		devbox.vm.provider "virtualbox" do |vb|
    		  vb.memory = 4096
    		  vb.cpus = 2
    		end
    		devbox.vm.provider "hyperv" do |h|
    		  h.memory = 4096
    		  h.cpus = 2
    		end
	end
end
