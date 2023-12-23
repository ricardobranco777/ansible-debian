
I use this playbook to install the following on my Raspberry Pi 4b & 5 running Ubuntu 23.10 & Debian 12:
 - Docker CE
 - Podman
 - NFS / Samba
 - Golang from upstream
 - vlc to connect to BlueTooth speakers

Check:
`ansible-playbook -v -C -i inventory main.yml`

Run with:
`ansible-playbook -v -i inventory main.yml`

NOTES:
  - passwordless sudo for pi user is disabled. Make sure you set a password for root before running this.
