#WORK IN PROGRESS
This project is under current development an not ready for usage

#openvpn-server
an automated openvpn-server-deployment using ansible

#requirements
- ansible 2.x
- vagrant

#usage
1. clone the repository
2. enter the vagrant folder `cd ./vagrant`
3. run `vagrant up`
4. enter the ansible folder `cd ../ansible`
5. run `ansible-playbook playbook.yml --inventory=inventory-virtualbox.ini`
