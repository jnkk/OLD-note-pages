---
title: Index for Personal Notes
tags: index
---


## [[Learning]]

Go to the directory vault/note-pages/content
Edit the index.md file

## Before stating the server

New home-manager, erases the nodejs module from bashrc.  
So run this first.  

```bash
nix-shell -p yarn yarn2nix nodejs
```

## Start the server

```bash
npx quartz build --serve
```

## Resync with github pages

```bash
npx quartz sync --no-pull
```
  
## [[Docker]](./Docker/Docker.md)  

## [[Blogs]](/Blog/Blog001.md)


### TODO

Customizing the "front page" to display foldered files

#### This is a blank Quartz installation.

See the [documentation](https://quartz.jzhao.xyz) for how to get started

Or see the note-pages directory
