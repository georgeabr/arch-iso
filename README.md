# arch-iso
### What it does
Builds an updated Archlinux ISO, with added packages and a custom installer.  

### How to download
Download the latest ISO from [releases](https://github.com/georgeabr/arch-iso/releases), assets.  
File names should be like this - `archlinux-2025.05.28-x86_64.iso`.
### How to use
Use `bash arch.sh` to start the custom installer.  
```bash
bash arch.sh
```
Installation is logged to a timestamped file, for example `install-20250418_1431.log`.
Use `tail -f` to monitor installation from another console.
```bash
tail -f install-20250418_1431.log
```
### Connect via SSH from another computer
- set password for `root` user from live ISO with `passwd`
- get IP address with `ip a`
- connect from other computer:
`ssh root@ip-address`
