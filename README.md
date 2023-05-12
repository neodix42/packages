### Install RPM (yum)
```
cat > /etc/yum.repos.d/ton.repo << EOF
[ton]
name=Ton
baseurl=https://neodix42.github.io/rpm-repo/rpm
enabled=1
type=rpm
gpgcheck=0
EOF
```
```
yum install ton
```

### Install AUR (pamac)
```
pamac build ton-bin
```