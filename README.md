### Install RPM (yum)
```
sudo bash -c 'cat > /etc/yum.repos.d/ton.repo << EOF
[ton]
name=Ton
baseurl=https://ton-blockchain.github.io/rpm-repo/rpm
enabled=1
type=rpm
gpgcheck=0
EOF'
```
```
yum install ton
```

### Install AUR (pamac)
```
pamac build ton-bin
```

### Install Windows binaries (choco)
```
choco install ton
```

### Install deb (apt)

```sh
sudo echo 'deb [trusted=yes] https://github.com/ton-blockchain/rpm-repo/releases/latest/download ./' > /etc/apt/sources.list.d/10-ton.list
sudo apt update
sudo apt install ton
```