Cheatsheet to remove Rust non-sense from Ubuntu 26.04:

```
# Disable password feeback
echo 'Defaults !pwfeedback' | sudo tee -a /etc/sudoers.d/nofeedback
# Remove sudo-rs
sudo apt remove -y sudo-rs
# Enable insults
echo Defaults insults | sudo tee -a /etc/sudoers.d/insults

```

```
# No stupid snap
sudo snap remove firefox firmware-updater prompting-client snap-store gnome-46-2404 mesa-2404 snapd-desktop-integration desktop-security-center gtk-common-themes
sudo snap remove core24 bare
sudo snap remove snapd
sudo apt remove firefox snapd
sudo apt purge firefox snapd
sudo apt-mark hold snapd
```

```
# Remove uutils and use good ol' GNU
sudo apt install --allow-remove-essential coreutils-from-gnu coreutils-from-uutils-
sudo apt remove rust-coreutils
sudo apt-mark hold rust-coreutils
```
