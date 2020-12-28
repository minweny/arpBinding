# arpBinding
arp -s 10.0.0.1 b0-39-56-d3-08-2d
sudo arp -s 10.0.0.1 b0:39:56:d3:08:2d
arp -d

Here is what I found and it works great

arp -s : access denied. On the default gateway

Here is what I used :

delete:

netsh interface ip delete neighbors "Network card name here" "Gateway.IP.goes.here"
Add:

netsh interface ipv4 add neighbors "Wi-Fi 2" 10.0.0.1 b0-39-56-d3-08-2d

netsh interface ipv4 delete neighbors "Wi-Fi 2" 10.0.0.1 b0-39-56-d3-08-2d
