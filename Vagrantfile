# -*- mode: ruby -*-
# vi: set ft=ruby :
VAGRANT_VERSION = 2
Vagrant.configure(VAGRANT_VERSION) do |config|
	config.vm.define "vulture" do |server|
		server.vm.box = "hashicorp/precise64"
		server.vm.hostname = "vulture"
		server.vm.provision :ansible do |ansible|
			ansible.playbook = "test.yml"
		end
	end
end
