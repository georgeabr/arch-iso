# arch-iso
### What it does
Builds an updated Archlinux ISO, with added packages.  

### How to download
Download the latest ISO from [releases](https://github.com/georgeabr/arch-iso/releases), assets.  
File names should be like this - `archlinux-2025.05.28-x86_64.iso`.
### How to use
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
