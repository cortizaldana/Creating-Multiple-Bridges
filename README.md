# Creating-Multiple-Bridges

# What Is The Point Of Creating A Bridge?

- TO implement network segmentation
- Each bridge will act like a network/subnet
- Each bridge will host different services for our production like enviornement 
- From a cost standpoint, this is the best way to go


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
