# okd-on-proxmox

inspired by https://github.com/hagen-bauer/Ansible-4-Openshift-on-Proxmox

## Environment
+ EdgeOS router as DHCP server
+ PiHole as DNS server (*.apps.\<cluster-id\>.\<domain\> record must be set manually, can't be set via API) 
+ Proxmox cluster with three nodes with proxmoxer python modul installed
+ Ansible playbooks are executed on infra VM (tested with Rocky Linux 8) hosting tftp server, ha proxy as loadbalancer, apache webserver for ignition files
