
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
`ansible-playbook -v -C -i inventory main.yml`

Run with:
`ansible-playbook -v -i inventory main.yml`

NOTES:
  - passwordless sudo for pi user is disabled. Make sure you set a password for root before running this.

Remove snapd from Ubuntu:

```
sudo snap remove thunderbird firefox snapd-desktop-integration snap-store gtk-common-themes gnome-42-2204 core22 bare snapd
sudo apt remove -y snapd
sudo rm -rf /var/lib/snapd/
```
