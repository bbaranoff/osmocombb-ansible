# osmocom-ansible

work at thursday 2018/04/19

apt dist-upgrade

wget http://kernel.ubuntu.com/~kernel-ppa/mainline/v4.15/linux-headers-4.15.0-041500_4.15.0-041500.201802011154_all.deb

wget http://kernel.ubuntu.com/~kernel-ppa/mainline/v4.15/linux-headers-4.15.0-041500-generic_4.15.0-041500.201802011154_amd64.deb

wget http://kernel.ubuntu.com/~kernel-ppa/mainline/v4.15/linux-image-4.15.0-041500-generic_4.15.0-041500.201802011154_amd64.deb

dpkg -i *.deb

update-grub

reboot on linux image 4.15 (in advanced options)
Check if new Kernel has been installed with command:

uname -r

4.15.0-041500-generic

cd /lib/modules/4.15.0-041500-generic/

ln -s /usr/src/linux-headers-4.15.0-041500 source

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


