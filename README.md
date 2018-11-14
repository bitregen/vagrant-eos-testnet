# Vagrant development environment for EOS testnet

This project allows anyone to set up a local EOS testnet development environment, on any operating system, within an Ubuntu 18.04 virtual machine. 

## Install

#### 1. Download and install VirtualBox and Vagrant 
[Download VirtualBox](https://www.virtualbox.org/wiki/Downloads) for your operating system.  
[Download the Vagrant installer](https://www.vagrantup.com/downloads.html) for your operating system.

#### 2. Clone this git repository 
```
git clone https://github.com/bitregen/vagrant-eos-testnet.git
```

#### 3. Start Vagrant
```
vagrant up
```

#### 4. ssh into your virtual machine
```
vagrant ssh
```

## TODO
1. Open network ports for EOS API endpoints
2. Install vagrant share for ngrok 
3. Confiugure chef for vim, git, bat, and other accessories

## Special thanks
Special thanks goes to the [UserFrosting](https://www.userfrosting.com/) crew for being awesome and adopting Vagrant. 
