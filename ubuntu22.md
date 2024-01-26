# Install Microsoft Edge

<https://www.windowscentral.com/software-apps/how-to-install-microsoft-edge-on-linux>


Debian
```
curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg

sudo install -o root -g root -m 644 microsoft.gpg /usr/share/keyrings/

sudo sh -c 'echo "deb [arch=amd64 signed-by=/usr/share/keyrings/microsoft.gpg]
https://packages.microsoft.com/repos/edge stable main" > /etc/apt/sources.list.d/microsoft-edge-beta. List'

sudo rm microsoft.gpg

sudo apt update

sudo apt install microsoft-edge-beta
```


# Make sudo Remember password for longer

```
sudo visudo
```

add ```Defaults        timestamp_timeout=300``` at the end


# Auto mount drive on booting the machine

```
sudo vim /etc/fstab
```

add ```/dev/{drive_name}      /media/path/to/mount   ext4   defaults   0   0```
