To run khanakhazana, 

    git clone http://github.com/fungibleclouds/khanakhazana.git	
    cd khanakhazana

Get these submodules using

    git submodule init
    git submodule update

    vagrant up

I cloned these inside cookbooks folder:

* apt https://github.com/opscode-cookbooks/apt
* mysql https://github.com/opscode-cookbooks/mysql
* OpenSSL https://github.com/opscode-cookbooks/openssl
* build-essential https://github.com/opscode-cookbooks/build-essential

	
http://vagrantup.com/v1/docs/provisioners/chef_solo.html	
http://vagrantup.com/v1/docs/troubleshooting.html
http://www.cyberciti.biz/faq/howto-install-kernel-headers-package/





This was created by 

git submodule add https://github.com/opscode-cookbooks/apt.git cookbooks/apt
git submodule add https://github.com/opscode-cookbooks/build-essential.git cookbooks/build-essential
git submodule add https://github.com/opscode-cookbooks/openssl.git cookbooks/openssl
git submodule add https://github.com/opscode-cookbooks/mysql.git cookbooks/mysql
