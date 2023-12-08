# Ansible_lamp_drupal
Ansible Lamp with Drupal Vagrant and Parallels configuration

macOS: Sonoma 14.1.1

Vagrant Box: luminositylabsllc/bento-ubuntu-20.04-arm64

Parallels: 19.1.1

Installation via GeerlingGuy roles:
	- Install roles with requiremensts file:
		$ ansible-galaxy install -r role_play/role_requirements.yml
	- run the playbook with your inventory file:
		$ ansible-playbook -i <path to your inventory> role_play/role_playbook.yml


ATTENTION
  1. If you are on local machine you have to add "drupal_test_conf:" path in vars.ini
  2. Run command to install roles with -c value (to ignore certificares) or install them with your own certificates if { SSL: CERTIFICATE_VERIFY_FAILED } appears.

links: 2nd edition of Ansible for DevOps Jeff Geerling
