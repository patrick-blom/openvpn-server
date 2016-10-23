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

#usefull informations
- You can configure the openvpn users using the `easy_rsa_clients` variable inside the playbook.yml . Add as much as you want.
- Ansible will generate the `.ovpn` client files in /root/clients/nameOfYourClient.
- The `.ovpn` files contain all necessary client informations.
- If you want to use the roles on an other server create an new inventory file and change the `openvpn_hostip` variable inside the playbook.yml
