# IoT-IP-Blocklist

I found ip address using following logs in Asus Router:


```
iptables -I FORWARD -s 192.168.50.221 -m state --state NEW -j LOG --log-prefix "New outbound: "
iptables -I FORWARD -d 192.168.50.221 -m state --state NEW -j LOG --log-prefix "New inbound: "
```
