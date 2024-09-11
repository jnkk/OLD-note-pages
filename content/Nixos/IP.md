# connect to local vm
ssh jnkk@192.168.122.148

## useful commands
  
```
sudo nixos-rebuild switch --flake .
```

## update nix flake lock file 

```
nix flake update
```

## update home-manager

```
home-manager switch --flake .
```

## mynixos search packages website

nixpkgs options are in configuration.nix
home-manager / option are in home-manager
