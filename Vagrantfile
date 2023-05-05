Vagrant.configure("2") do |config|
  
### Nginx VM ###
  config.vm.define "web01" do |web01|
    web01.vm.box = "ubuntu/bionic64"
    web01.vm.hostname = "web01"
    web01.vm.network "private_network", ip: "192.168.56.19"
    web01.vm.provider "vmware_desktop" do |vmware|
      vmware.gui = true
      vmware.allowlist_verified = true
    web01.vm.provision "shell", path: "nginx.sh"   
    end
  end 
  
end  