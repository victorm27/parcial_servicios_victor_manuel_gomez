Vagrant.configure("2") do |config|
 if Vagrant.has_plugin? "vagrant-vbguest"
 config.vbguest.no_install = true
 config.vbguest.auto_update = false
 config.vbguest.no_remote = true
 end
 config.vm.define :cliente do |cliente|
 cliente.vm.box = "generic/centos9s"
 cliente.vm.network :private_network, ip: "192.168.50.2"
 cliente.vm.hostname = "cliente"
 end
 config.vm.define :servidor do |servidor|
 servidor.vm.box = "generic/centos9s"
 servidor.vm.network :private_network, ip: "192.168.50.3"
 servidor.vm.hostname = "servidor"
 end
end
