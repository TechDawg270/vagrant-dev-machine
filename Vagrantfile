Vagrant.configure(2) do |config|
	config.vm.define "vagrant-dev-machine" do |devbox|
		devbox.vm.box = "ubuntu/xenial64"
		if File.exist?("~/.aws")
			config.vm.synced_folder "~/.aws", "/home/ubuntu/.aws"
		end
		if File.exist?("~/Development")
			config.vm.synced_folder "~/Development", "/home/ubuntu/Development"
		end
		devbox.vm.provision "shell", path: "scripts/install.sh"
		devbox.vm.provider "virtualbox" do |v|
			v.memory = 1024
			v.cpus = 2
		end
	end
end
