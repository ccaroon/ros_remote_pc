# ROS - Remote PC
Vagrant VM for the Remote PC part of the ROS Environment.

## Prerequisites
1. Install `vagrant`
    - `vagrant plugin install vagrant-hostmanager`
2. Install `VirtualBox`
3. Install Ansible: `pip install ansible`


## Start Up
0. Edit `ros-local-setup.yml`
    - change `vars:user` to your preferred username
1. `vagrant up`

## Install ROS & Friends
0. `ssh ros.local`
1. `cd ros`
2. `./scripts/1_install_ros.sh`
2. Reboot VM: `vagrant reload`
3. `./scripts/2_install_deps.sh`
4. `./scripts/3_build.sh`
