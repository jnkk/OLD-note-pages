---
title: Beginning of NixOS Setups
tags: homelab, linux, nix, nixos
---

# First steps

The base of nixOS is in /etc/nixos.
There are 2 files, configuration.nix and hardware-configuration.nix

DO NOT MOVE THESE FILES.
The command
```
sudo nixos-rebuild switch
```
will be defaulted in /etc/nixos
Changes won't happend


Enable ssh, git, curl in configuration.nix

```
services.openssh.enable = true;

environment.systemPackages = with pkgs; [
    wget git curl
  ];
```

Add this to configuration.nix
```
nix.settings.experimental-features = [ "nix-command" "flakes" ];
```

What these do is "replacing" the channels command, which are the defaults.
To the flakes "channels".

The difference is channel default uses sudo, flakes does not.

## With hardships, zsh is installed and made the default shell

## Next step is emacs or neovim
