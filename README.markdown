To run khanakhazana, 

    git clone http://github.com/fungibleclouds/khanakhazana.git	
    cd khanakhazana

Get needed submodules

    git submodule init
    git submodule update

Fire up vagrant VM

    vagrant up

Fire up vagrant without provisioining (so as to run chef-solo manually if needed)

    vagrant up --no-provision
	vagrant ssh
	sudo chef-solo -c /vagrant/solo.rb -j /vagrant/node.json

Note: `/vagrant` maps back to the host location `khanakhazana` from where it picks up `solo.rb` and `node.json`	

READINGS
	
* http://vagrantup.com/v1/docs/provisioners/chef_solo.html	
* http://vagrantup.com/v1/docs/troubleshooting.html

I added these submodules inside cookbooks folder:

    git submodule add https://github.com/opscode-cookbooks/apt.git cookbooks/apt
    git submodule add https://github.com/opscode-cookbooks/build-essential.git cookbooks/build-essential
	git submodule add https://github.com/opscode-cookbooks/openssl.git cookbooks/openssl
	git submodule add https://github.com/opscode-cookbooks/mysql.git cookbooks/mysql
