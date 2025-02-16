Quick hacks like this:

```
user@personal:~$ cat  QubesIncoming/dom0/qrexectimeoutfixattempt.sh 
#!/bin/bash
#
# this is not yet solution, but an attempt (based on google search)
#
echo "sudo qvm-prefs --set sys-net qrexec_timeout 90"
sudo qvm-prefs --set sys-net qrexec_timeout 90
echo "sudo qvm-prefs --set sys-firewall qrexec_timeout 90"
sudo qvm-prefs --set sys-firewall qrexec_timeout 100
echo "sudo qvm-prefs --set sys-whonix qrexec_timeout 100"
sudo qvm-prefs --set sys-whonix qrexec_timeout 100
echo "sudo qvm-prefs --set sys-usb qrexec_timeout 90"
sudo qvm-prefs --set sys-usb qrexec_timeout 90

user@personal:~$ 

```
