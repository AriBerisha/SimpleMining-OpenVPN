# Mining-OpenVPN
Easily install VPN on Ubuntu 18.04  Mining Based OS's

# Clone the Repository!
```
git clone https://github.com/AriBerisha/SimpleMining-OpenVPN.git
```

# Add this to your ovpn file under verb 
```
script-security 2
up /etc/openvpn/update-systemd-resolved
down /etc/openvpn/update-systemd-resolved
down-pre
```
If using NordVPN
```
auth-user-pass /etc/openvpnservers/login.conf
script-security 2
up /etc/openvpn/update-systemd-resolved
down /etc/openvpn/update-systemd-resolved
down-pre
```


# Instructions
Tested on Ubuntu 18.04 Based Mining OS's
Should work on Debian 11 and Ubuntu 20.04


1. To be safe from any errors run the file as sudo
2. Run the following commands on the directory where the bash script is
```
    cd SimpleMining-OpenVPN
```

```
    sudo chmod u+x simpleminingvpn.sh
```

```
    sudo ./simpleminingvpn.sh
```



3. Insert link to ovpn file, script uses wget and you can use something like Dropbox,Drive,Transfer.sh
4. Reboot if any problems and you're set!
5. If you run into issues with network, to undo just do systemctl disable simpleminingvpn.service
