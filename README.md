# ansible-hosts-cfg
[hq]
hq-rtr ansible_host=172.16.4.2 ansible_user=net_admin ansible_password=P@ssw0rd ansible_connection=network_cli ansible_network_os=ios
br-rtr ansible_user=net_admin ansible_password=P@ssw0rd ansible_connection=network_cli ansible_network_os=ios
hq-cli ansible_ssh_user=student
hq-srv ansible_ssh_user=sshuser ansible_port=2024

nano /etc/ansible/ansible.cfg
[defaults]
interpreter_python = /usr/bin/python3

dnf install sshpass
dnf install pip
pip install ansible-pylibssh
