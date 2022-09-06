Vagrant.configure("2") do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://vagrantcloud.com/search.
  config.vm.box = "ubuntu/focal64"
# # prometheus
config.vm.define "prometheus" do |app|
app.vm.hostname = "prometheus"
app.vm.provider :virtualbox do |v|
v.memory = 4092
end
app.vm.network :private_network, ip: "192.168.60.100"
end
# # Node 1.
config.vm.define "node1" do |app|
app.vm.hostname = "node1"
app.vm.network :private_network, ip: "192.168.60.4"
end
 # # Node 2.
config.vm.define "node2" do |app|
app.vm.hostname = "node2"
app.vm.network :private_network, ip: "192.168.60.5"
end
end
