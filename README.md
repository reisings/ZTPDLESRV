This vagrant project encompasses several different services for Juniper products.

1: DHCP and HTTP daemons working together for Zero Touch Provisioning (ZTP)
2: TFTP server (In case you need one)
3: Cloud Analytics Engine (CAE)
4: Data Learning Engine (DLE) for SFLOW collection and Network Analysis with Network Director
5: Apache Web Services with DAV turned on so this can be used for file repo
6: Could also be used as a Jump Box as openssh is used
7: This box has Ansible and PyEZ enabled along with some basic playbooks (Ready to go)


Future revisions:

- Plan on adding FreeRadius to use this box as a Radius Test server

To launch this box you can download it directly using git and then use vagrant up to start it in the VirtualBox Hypervisor.



