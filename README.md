# osmocom-ansible

work at thursday 2018/04/19

apt dist-upgrade

apt install openssh-server ansible

cd /root

git clone https://github.com/bbaranoff/osmocombb-ansible test

cp /root/test/hosts /etc/ansible/hosts

cp /root/test/sshd_config /etc/ssh/sshd_config

ssh-keygen

service ssh restart

ssh-copy-id localhost

ansible all -m ping

if it answer pong you're good

cd /root/test/

ansible-playbook osmocombb.yml


