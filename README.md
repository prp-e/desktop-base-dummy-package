# Debian's `desktop-base` dummy package

## Introduction

If you have ever tried to make a desktop system based on [Debian GNU/Linux](https://debian.org) you have faced the huge problem of `desktop-base` package, where it installs all unnecessary branding of the Debian systems. It is okay when you are setting up a personal Debian system, but for distribution developers, it can get a little too annyoing. Now, it is time to revise it and make a _dummy_ package for `desktop-base`. 

## Packages

For this particular project you only need `equivs` package. You just need to do this: 

```
apt update
apt install equivs
```

## How to use this repository

1. Clone this repository
2. Move the folder of the repository
3. Run `equivs-build desktop-base`
4. Running `dpkg -i` command to install the resulting package.