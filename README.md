Nginx installation on CenOS6
=========

Installs EPEL repo (because there is no Nginx in standard CentOS repo) and Nginx. Only installs
Nginx if OS is CentOS and version major is 6.

Example Playbook
----------------

Usage:  ansible-playbook -i /etc/ansible/invs /etc/ansible/roles/testrole.yml -e "ROLE=<role>" -e "TARGETHOST=<i.p.add.ress>"

- hosts:  '{{TARGETHOST}}'
  user:    test
  become: yes
  become_method: sudo

  roles:
  - { role: '{{ROLE}}' }


Author Information
------------------

Serge G, g2009j at gmail