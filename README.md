# my-working
Sample 1 android config ovpn
Get for dns 

auth-user-pass
client
dev tun
proto tcp
remote 139.99.90.36 443
remote 
www.googleapis.com.abdhan.pointdns.pro 443
persist-key
persist-tun
pull
resolv-retry infinite
nobind
user nobody
comp-lzo
remote-cert-tls server
verb 3
mute 2
connect-retry 5 5
connect-retry-max 8080
mute-replay-warnings
redirect-gateway def1
script-security 2
cipher none
auth none
<ca>

Sample 2 
Get for http proxy 

client
proto tcp-client
remote 51.158.146.40 443
http-proxy-option CUSTOM-HEADER Host
google.com
http-proxy 51.158.146.40 8080
auth-user-pass 
dev tun
resolv-retry infinite
nobind
persist-key
persist-tun
remote-cert-tls server
auth SHA256
auth-nocache
cipher AES-128-GCM
tls-client
tls-version-min 1.2
tls-cipher TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256
ignore-unknown-option block-outside-dns
setenv opt block-outside-dns 
verb 3
<ca>

Sample 3
Get http proxy

client
proto tcp-client
remote 66.94.97.238 443
auth-user-pass
dev tun
resolv-retry infinite
nobind
persist-key
persist-tun
remote-cert-tls server
auth SHA256
auth-nocache
cipher AES-128-GCM
tls-client
tls-version-min 1.2
tls-cipher TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256
ignore-unknown-option block-outside-dns
setenv opt block-outside-dns
verb 3

http-proxy 66.94.97.238 8080
http-proxy-option CUSTOM-HEADER CONNECT HTTP/1.0
http-proxy-option CUSTOM-HEADER Host group.calendar.google.com.calendar.google.com.activity.mobilelegends.com.www.googlevideo.com
http-proxy-option CUSTOM-HEADER X-Online-Host group.calendar.google.com.calendar.google.com.activity.mobilelegends.com.www.googlevideo.com
http-proxy-option CUSTOM-HEADER X-Forward-Host group.calendar.google.com.calendar.google.com.activity.mobilelegends.com.www.googlevideo.com
http-proxy-option CUSTOM-HEADER Connection:Keep-Alive

<auth-user-pass>
tcpvpn.com-abdya22
abd112
</auth-user-pass>

Sample 4 
http 

client
dev tun
proto tcp
remote 194.233.73.107 110
http-proxy 127.0.0.1 8989
resolv-retry infinite
nobind
tun-mtu 1500
tun-mtu-extra 32
mssfix 1450
persist-key
persist-tun
auth-user-pass
comp-lzo
reneg-sec 0
verb 3


