# Installing nix + home-manager

> [!TIP]
> Using alt + m to display markdown editing tools. Really handy.

Determinate Systems have a really good documentation (or starting point) for nix language

[Documentation link](https://determinate.systems/posts/determinate-nix-installer/)


```bash
curl --proto '=https' --tlsv1.2 -sSf -L https://install.determinate.systems/nix | sh -s -- install
```

[MyNixos](https://mynixos.com/) is a really good website to look up how the configurations are coded.

## Managing dotfiles

The *easy* way of learning is my configuring dotfiles, since you can *literally* add anything. Customizing is a different playing field.  
  
My first steps are configuring bash and neovim. VSCode as the main IDE is great and I'm used to it but really heavy in my current setup.

## How to install nixvim in home manager using Debian

In the `flake.nix` file, add code below in ***inputs***:

```nix
    nixvim = {
      url = "github:nix-community/nixvim";
      # If you are not running an unstable channel of nixpkgs, select the corresponding branch of nixvim.
      # url = "github:nix-community/nixvim/nixos-24.05";

      inputs.nixpkgs.follows = "nixpkgs";
    };
```  

it is in the where you declare your nixpkgs.url or home-manager url.  

I added nixvim to the output ***nixvim*** like in the same `flake.nix` file:

```nix
outputs = { self, nixpkgs, home-manager, nixvim, ... }:
```

And then you make the nixvim `default.nix` file:

```nix
    { ... }:
    {
        programs.nixvim = {
            enable = true;
        };
    }
```

test in the terminal: nvim

