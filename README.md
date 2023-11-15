
I use this playbook to install the following on my Raspberry Pi 4b running Debian 12:
 - Docker CE
 - Podman
 - NFS / Samba

Check:
`ansible-playbook -v -C -i inventory main.yml`

Run with:
`ansible-playbook -v -i inventory main.yml`
