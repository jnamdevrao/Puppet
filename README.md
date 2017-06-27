"# Puppet" 
Lab Setup Instructions

git clone this repository or download master.zip and unzip to the puppet-fundamentals-lab directory and cd to it.

Download the CentOS 6.5 Vagrant box to the puppet-fundamentals-lab directory.

Ensure the file is saved as centos65.box.

Add the CentOS 6.5 box you just downloaded: vagrant box add centos65-base centos65.box

Download the Ubuntu 14.04 Vagrant box to the same directory: http://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box

Add the Ubuntu box: vagrant box add trusty64 trusty-server-cloudimg-amd64-vagrant-disk1.box

Booting the Puppet Master Server

cd into the puppetmaster subdirectory and launch the VM: vagrant up

Once the machine is booted, SSH into it: vagrant ssh

Windows 2008 R2 ISO

http://www.microsoft.com/en-us/download/details.aspx?id=11093
-----------------------------------------------------------------------------------------------------------------------------------------
"Installing Apache and Passenger" clip of the "Installing and Configuring the Puppet Master" module:

(Optional) From your host machine, take a snapshot: vagrant snapshot save puppetmaster
---------------------------------------------------------------------------------------
Install the following: 
sudo gem install rake --version 10.4.2 
sudo gem install rack --version 1.6.0 
sudo gem install passenger --version 4.0.56
sudo gem install daemon_controller --version 1.2.0
------------------------------------------------------------------------------------------------------------------------------------------
Install the Passenger Apache module: 
sudo passenger-install-apache2-module

