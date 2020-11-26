Dell OS10 Ansible Environment

This has been built to simply and speed up your very first Ansible + OS10 project

TESTED with Ansible 2.9.13 and Python 3.6.9

# Prerequisites: 

- Dell OS10.5.x physical or Virtual Environment i.e., with GNS3
- GNS3project will be share when the project is completed
- Get an Ubuntu 18.04 fresh installed.

Run initialize.sh on your Ubuntu it will install all software needed and a very basic Config_host name Ansible Playbook. 

Run the following commands to install git and the the very first file.


sudo apt install git

git clone https://github.com/val3r1o/startupdellos10ansible.git

cd startupdellos10ansible

sudo chmod 755 initialize.sh

ls

./initialize.sh

source ~/opt/dellos10env/bin/activate

ansible --version

ansible-playbook -i inventory conf-hostname.yml
