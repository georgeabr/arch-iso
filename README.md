# arch-iso
### What it does
Builds an updated Arch Linux ISO, with added packages, a custom installer, and `diskviz` for disk partitioning.

### How to download
Download the latest ISO from [releases](https://github.com/georgeabr/arch-iso/releases), assets.
File names should be like this - `archlinux-cli-2026.08.13-x86_64.iso` (or `archlinux-xfce-2026.08.13-x86_64.iso` for the XFCE build).

### How to use
On login, a banner points you to the two custom tools. `arch.sh` is already executable, so just run it directly - no `chmod` needed:
```bash
./arch.sh
```
Installation is logged to a timestamped file, for example `install-20260813_1431.log`.
Use `tail -f` to monitor installation from another console.
```bash
tail -f install-20260813_1431.log
```

### Partitioning with `diskviz`
Before running the installer, use `diskviz` to inspect and partition your disks:
```bash
diskviz
```

### Connect via SSH from another computer
- set password for `root` user from live ISO with `passwd`
- get IP address with `ip a`
- connect from other computer:
`ssh root@ip-address`

### Use `XFCE` releases for a graphical installation
- use `startx` from the console to get to the GUI
- use `gparted`, or `diskviz` from a terminal, to partition disks
- from a console:
```bash
./arch.sh
```
