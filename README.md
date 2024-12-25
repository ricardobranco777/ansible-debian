
I use this playbook to install the following on my Raspberry Pi 4b & 5 running Ubuntu 24.04 & Debian 12:
 - Docker CE
 - Podman
 - NFS / Samba
 - Golang from upstream
 - vlc to connect to BlueTooth speakers

Enable SSH:

```
sudo apt install openssh-server
sudo systemctl --enable now ssh
```

Check:
`ansible-playbook -v -C -i inventory.yml main.yml`

Run with:
`ansible-playbook -v -i inventory.yml main.yml`
