Vagrant.configure("2") do |config|


    config.vm.define "ansible-server" do |client|
    	client.vm.box = "bento/centos-7.4"
    	client.vm.network "private_network", ip: "192.168.50.2"
    	client.vm.synced_folder "C:/Users/"+ENV["user"]+"/Desktop", "/ansible"
    end
    
    (1..4).each do |i|
        config.vm.define "server#{i}" do |client|
            client.vm.box = "bento/centos-7.4"
            client.vm.network "private_network", ip: "192.168.50.#{i+2}"
        end
    end

end

