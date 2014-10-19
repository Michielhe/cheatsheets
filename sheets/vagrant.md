# Vagrant Cheat Sheet

Useful links:
* **Vagrant** 
* Vbox documentation: https://docs.vagrantup.com/v2/virtualbox/boxes.html
* Documentation for Ansible: http://docs.ansible.com/guide_vagrant.html
* Example download: https://github.com/bertvv/vagrant-example (git clone git@github.com:bertvv/vagrant-example.git)

Create Vagrant Base Box:
* Make base VM in Virtualbox (see virtualbox.md)
* vagrant package --base <name_of_vm_in_virtualbox>
* vagrant box add <name_of_vm_in_virtualbox> <.box_file_location>
* Edit vagrantfile (see VagrantFile file)
