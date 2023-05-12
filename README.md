# TON installation packages for various operating systems

These packages are based on the latest binary artifacts which automatically downloaded from https://github.com/ton-blockchain/ton  

### Install RPM (yum)
```
sudo bash -c 'cat > /etc/yum.repos.d/ton.repo << EOF
[ton]
name=Ton
baseurl=https://neodiX42.github.io/packages/rpm
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
# currently unavailable since still in the review at https://community.chocolatey.org/
choco install ton
```

### Install deb (apt)

```
sudo bash -c "echo 'deb [trusted=yes] https://github.com/neodiX42/packages/releases/latest/download ./' > /etc/apt/sources.list.d/10-ton.list"
sudo apt update
sudo apt install ton
```