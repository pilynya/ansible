# ansible
[hq]
hq-srv ansible_ssh_user=sshuser ansible_port=2025
hq-rtr ansible_user=net_admin ansible_password=P@ssw0rd ansible_connection=network_cli ansible_network_os=iso
[routers]
hq-rtr ansible_user=net_admin ansible_password=P@ssw0rd ansible_connection=network_cli ansible_network_os=iso
br-rtr ansible_user=net_admin ansible_password=P@ssw0rd ansible_connection=network_cli ansible_network_os=iso
[info]
hq-cli ansible_ssh_user=student
hq-srv ansible_ssh_user=sshuser ansible_port=2025

nano /etc/ansible/ansible.cfg
[defaults]
interpreter_python = /usr/bin/python3

dnf install sshpass
dnf install pip
pip install ansible-pylibssh
