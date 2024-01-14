---
author: nam truong
pubDatetime: 2022-09-23T15:22:00+11:00
modDatetime: 2024-01-14T21:00:00+11:00
title: how to install apps on arch linux
slug: how to install apps on arch linux
featured: true
draft: false
description:
  how to install apps on arch linux
tags:
  - arch linux
  - CLI(command line)
---
# Installing apps on arch linux
This guide will walk you through the steps of installing applications on Arch Linux using the command line interface (CLI). Arch Linux uses the **'pacman'** package manager, renowned for its simplicity and efficiency.
## Updating the Package Database
Before installing any new packages, it's a good practice to update the package database. This ensures you're accessing the latest versions of packages. Run the following command:
```bash
sudo pacman -Sy
```
## Installing Packages
To install a package, you'll use the __'pacman -S'__ command followed by the package name. Here's the general syntax:
```bash
sudo pacman -S package_name
```
Replace __'package_name'__ with the actual name of the package you wish to install.
### Example
If you want to install the text editor __'nano'__, you would use:
```bash
sudo pacman -S nano
```
## Searching for Packages
If you're unsure of the exact package name, you can search the Arch repository using:
```bash
pacman -Ss keyword
```
Replace __'keyword'__ with a relevant term or name related to the package you're searching for.
## Updating Packages
To update all your packages to their latest versions, use:
```bash
sudo pacman -Syu
```
## Removing Packages
To remove an installed package, use:
```bash
sudo pacman -R package_name
```
Replace __package_name__ with the name of the package you wish to remove.
## Cleaning the Package Cache
Over time, __'pacman'__ stores downloaded packages in a cache. This can take up a lot of space, and you may want to clean it occasionally. To remove all cached packages that are not currently installed, and the database is synced, use:
```bash
sudo pacman -Sc
```
## Conclusion
Using __'pacman'__ to manage packages on Arch Linux is straightforward. Remember to regularly update your system and clean the cache to keep your system efficient and up-to-date.