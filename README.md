# CyberED
A repository created for educational purposes


ansible lab 1
Скопировать в корень директории папку labs и ключи для ssh

Сконфигурировать vagrant.config + проверить корректность настроек созданных VM и заданным настрокам в конфиге.

Установить Ansible + сконфигурировать playbook

Проверить доступность хостов
ansible -i labs/hosts all -m ping

Выполнить playbook
ansible-playbook -i labs/hosts labs/site.yaml -D

Выполнить playbook c паролем для root 
ansible-playbook -i labs/hosts labs/site.yaml -D --extra-vars "ansible_sudo_pass=..."
