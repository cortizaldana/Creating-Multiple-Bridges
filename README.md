# Creating-Multiple-Bridges

# Commands Issued To Create A Bridge

```
nmcli con add con-name br1-isl type bridge ifname br1-isl ipv4.method manual ip4 10.0.0.1/24 connection.zone isl
```
```
nmcli con add con-name br2-isl type bridge ifname br1-isl ipv4.method manual ip4 10.0.0.1/24 connection.zone isl
```
```
firewall-cmd --new-zone isl --permanent
```
