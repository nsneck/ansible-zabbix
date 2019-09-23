# A Zabbix installation exercise with Ansible

Do not actually use this in production, the MySQL root credentials issue
for example would have to be solved in a better way (preferably by not
trying to make things work with Ansible 2.5 and MySQL 5.7 with the new
root authentication plugin, as was done with this project.)

usage:

`ansible-playbook -i hosts -k --ask-become-pass zbx-server-install.yml`
Installs and configures the Zabbix server on given host(s).
Leads you to the Zabbix web configuration page.
Only tested to work under Ubuntu 18.04, definitely not working on
non-Debian based systems.
