# ansible-chef - setup chef over ansible

## Sample Run :
- setup server before register to chef server :
`ansible-playbook -i inventories/client_hosts -l elk.jcolab.lan playbooks/chef-client.yml --tags client-setup`

- registering server to chef server :
`ansible-playbook -i inventories/client_hosts -l elk.jcolab.lan playbooks/chef-client.yml --tags client-register`

## Reference :
https://tech.napsty.com/2016/08/integrating-chef-and-ansible.html
https://docs.chef.io/workstation/knife_bootstrap/
https://hendro-wibiksono.web.id/2022/02/11/cara-install-chef-infra-pada-almalinux-centos-8-rocky-linux-redhat-8/
