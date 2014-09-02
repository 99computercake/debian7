debian7
=======

Debian 7 Scripts for VPS &amp; SSH Seller by Yuri Bhuana


Autoscript Include:
===========================================

Service
-------
OpenSSH  : 22, 143
Dropbear : 443, 110, 109
Squid3    : 80, 8080 (limit to IP SSH)
OpenVPN  : TCP 1194 (client config : http://IPVPS/1194-client.ovpn)
badvpn   : badvpn-udpgw port 7300
nginx    : 81

Tools
-----
axel, bmon, htop, iftop, mtr, rkhunter, nethogs: nethogs venet0

Script
------
screenfetch
./ps_mem.py (Cek RAM)
./speedtest_cli.py --share (Speed Test VPS)
./bench-network.sh (Cek Kualitas VPS)
./user-login.sh (Monitoring User Login Dropbear, OpenSSH dan PPTP VPN)
./user-expired.sh (Auto Lock User Expire tiap jam 00:00)
./user-list.sh (Melihat Daftar User)
sh dropmon [port] contoh: sh dropmon 443

Fitur lain
----------
Webmin   : http://$MYIP:10000/
vnstat   : http://IPVPS/vnstat/ (Cek Bandwith)
MRTG     : http://IPVPS/mrtg/
Timezone : Asia/Jakarta (GMT +7)
Fail2Ban : [on]
IPv6     : [off]

Script Modified by Yuri Bhuana (fb.com/youree82, 0858 1500 2021)
Credit to Yurissh OpenSource
Thanks to Original Creator Kang Arie & Mikodemos

Log Instalasi --> /root/log-install.txt

VPS AUTO REBOOT TIAP 12 JAM, SILAHKAN REBOOT VPS ANDA !

===========================================



## ezpptp
========

A PPTP VPN setup script for a Debian/Ubuntu VPS (OpenVZ)

### To install the script, copy and paste this into your SSH client of choice:

	wget https://raw.github.com/cwaffles/ezpptp/master/ezpptp.sh
	chmod +x ezpptp.sh && ./ezpptp.sh

## Credits
- [cwaffles (me)](http://www.putdispenserhere.com/)
- [Denis](http://bluemodule.com/software/openvpn-install-script-for-openvz-vps/)
