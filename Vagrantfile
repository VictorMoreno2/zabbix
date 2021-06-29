machines = {
  'server1' => {'ip' => '10'},
  'server2' => {'ip' => '20'},
  'server3' => {'ip' => '30'}
}

Vagrant.configure("2") do |config|
  machines.each do |name,conf|
    config.vm.define name do |machine|
      config.vm.box = "ubuntu/focal64"
      machine.vm.network "private_network", ip: "10.0.0.#{conf['ip']}"
      end
      end
      end  
