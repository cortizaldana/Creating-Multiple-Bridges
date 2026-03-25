# PE-Creating-Multiple-Bridges

# Commands Issued To Create Multiple Bridges

```
nmcli con add con-name br1 type bridge ifname br1 ipv4.method manual ip4 10.0.0.1/24 connection.zone galileo
```
```
nmcli con add con-name br2 type bridge ifname br2 ipv4.method manual ip4 10.0.1.1/24 connection.zone galileo
```
```
firewall-cmd --new-zone galileo --permanent ; firewall-cmd --reload
```

# Video 
