# this is for debian 12, if another reinstall is needed

## change sourcelist. make a backup of the original file and copy and paste in /etc/apt 
deb http://deb.debian.org/debian bookworm main contrib non-free non-free-firmware
deb-src http://deb.debian.org/debian bookworm main contrib non-free non-free-firmware

deb http://deb.debian.org/debian-security bookworm-security main contrib non-free non-free-firmware
deb-src http://deb.debian.org/debian-security bookworm-security main contrib non-free non-free-firmware

deb http://deb.debian.org/debian bookworm-updates main contrib non-free non-free-firmware
deb-src http://deb.debian.org/debian bookworm-updates main contrib non-free non-free-firmware


## post debian 12 install to download
curl wget git micro btop build-essential cmake gcc

## other must to install not with apt
go rust

## best terminal by far is FISH
have to learn it.
if fish is set up. type this:
$ fish_config theme choose Tomorrow


## tutorial for installing QEMU/KVM
https://www.youtube.com/watch?v=GgAQw08zJzs

