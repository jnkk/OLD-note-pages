# this is for debian 12, if another reinstall is needed

## change sourcelist. make a backup of the original file and copy and paste in /etc/apt 

> [!]IMPORTANT
> Make sure to backup first and then edit the files

deb http://deb.debian.org/debian bookworm main contrib non-free non-free-firmware  
deb-src http://deb.debian.org/debian bookworm main contrib non-free non-free-firmware  

deb http://deb.debian.org/debian-security bookworm-security main contrib non-free non-free-firmware  
deb-src http://deb.debian.org/debian-security bookworm-security main contrib non-free non-free-firmware  

deb http://deb.debian.org/debian bookworm-updates main contrib non-free non-free-firmware  
deb-src http://deb.debian.org/debian bookworm-updates main contrib non-free non-free-firmware  


## post debian 12 install to download
```bash
sudo apt install curl wget git micro btop build-essential cmake gcc brew vscodium nvidia-tesla-470-driver
```
> []NOTE
> current setup is using a dell laptop that has a old nvidia  
> use-> nvidia-tesla-470-driver  
> nvidia-detect

## How to download and make use of personal notes

1. set your git username and email
```bash
git config --global user.name "<yourusername>"
git config --global user.email "<youruseremail>"
```

2. create ssh-key
```bash
ssh-keygen -t rsa
```

> [!]NOTE  
> using SUDO goes to the root user.

3. add ssh key to [github](https://github.com/settings/keys)  
4. download the GIT version and not the https. so the git push command works.


## other must to install not with apt
go rust cloudflare-warp speedtest-cli fast-cli 

## apps using BREW  
lazygit ruff

## install miniconda for shell-gpt
[miniconda](https://docs.anaconda.com/miniconda/miniconda-install/)  
Make sure to download sh their file. use bash command to install those.
last time I tried their failed because of the agreements.

## best terminal by far is FISH
have to learn it.
if fish is set up. type this:
$ fish_config theme choose Tomorrow


## tutorial for installing QEMU/KVM
[youtube](https://www.youtube.com/watch?v=GgAQw08zJzs)
or go to [chatgpt](https://chatgpt.com/)/[perplexity](https://www.perplexity.ai/)

"how to install qemu/kvm on debian 12"
