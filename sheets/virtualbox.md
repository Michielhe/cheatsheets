# Setup CentOS on Virtualbox

Source: https://www.youtube.com/watch?v=Kma_0BQUTLM&list=PL37738752AD3E0B3A
* Download & install Virtualbox: https://www.virtualbox.org/wiki/Downloads
* Download CentOS DVD: http://www.centos.org/download/
* Start Virtualbox
* New
..* Name: Centos7
..* Type: Linux
..* Version: Red Hat (64 bit)
* Rest default settings
* VM Settings -> Storage -> Under Controller: IDE, Empty -> CD Icon -> Select CentOS DVD iso
* VM Settings -> Network -> Second tab
..* Bridged adapter (so your PC can connect to the VM through the local network)
..* Host-Only Network (see below)
* Start VM
* Install CentOS (default settings work)
* Shutdown system
* Remove CentOS DVD from Storage


# Setup Host-Only network

Used for direct interface between VM and host machine
* File -> Preferences... -> Network -> Host-Only Networkds -> Add
* OK
* VM Settings -> Network -> Host-Only Network
* Test: ifconfig vboxnet0 (name of network in VirtualBox), 192.168.56.0/24

