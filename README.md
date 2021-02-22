# sysctl
sysctl

```
# Search value
sysctl -a | grep -i forward 

# Read value
sysctl net.ipv4.ip_forward
net.ipv4.ip_forward = 1

# Write value
sysctl -w net.ipv4.ip_forward = 1

# Persistent values => Add or Update values in /etc/sysctl.conf
net.ipv4.ip_forward = 1

# reload values
$ sysctl --system
ysctl --system
* Applying /etc/sysctl.d/10-console-messages.conf ...
kernel.printk = 4 4 1 7
* Applying /etc/sysctl.d/10-ipv6-privacy.conf ...
net.ipv6.conf.all.use_tempaddr = 2
...
```
