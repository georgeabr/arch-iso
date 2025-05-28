# arch-iso
Build an updated Archlinux ISO, with added packages.  
Use `bash arch.sh` to start the custom installer.  
```bash
bash arch.sh
```
Use `tee` to also log onscreen installation to a file.
```bash
bash arch.sh 2>&1 | tee install-$(date +%Y%m%d_%H%M).log
```
### Connect via SSH from another computer
- set password for `root` user from live ISO with `passwd`
- get IP address with `ip a`
- connect from other computer:
`ssh root@ip-address`
