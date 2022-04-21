# dockerswarm

Vagrant.configure("2") do |config|
config.vm.define "master" do |vm1|
vm1.vm.box = "centos/8"
vm1.vm.hostname = 'master'
vm1.vm.box_url = "centos/8"
vm1.vm.network "public_network", bridge: "en0: Wi-Fi (AirPort)", auto_config: false
end
config.vm.define "worker1" do |vm2|
vm2.vm.box = "centos/8"
vm2.vm.hostname = 'worker1'
vm2.vm.box_url = "centos/8"
vm2.vm.network "public_network", bridge: "en0: Wi-Fi (AirPort)", auto_config: false
end
config.vm.define "worker2" do |vm3|
vm3.vm.box = "centos/8"
vm3.vm.hostname = 'worker2'
vm3.vm.box_url = "centos/8"
vm3.vm.network "public_network", bridge: "en0: Wi-Fi (AirPort)", auto_config: false
end
config.vm.define "worker3" do |vm4|
vm4.vm.box = "centos/8"
vm4.vm.hostname = 'worker3'
vm4.vm.box_url = "centos/8"
vm4.vm.network "public_network", bridge: "en0: Wi-Fi (AirPort)", auto_config: false
end
end
