# My NixOS Configurations

This repository contains my personal NixOS configuration files and customizations. NixOS is a unique Linux distribution that uses the Nix package manager and a declarative configuration model.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Customization](#customization)

## Introduction

This repository serves as a backup and version-controlled history of my NixOS configurations. It includes settings for system packages, user environments, and various services.

## Installation

To use my NixOS configurations, clone this repository and follow these steps:

```bash
git clone https://github.com/xanmoy/nixos-config.git
cd nixos-config
```

1. Copy the configuration files to the appropriate directory:

```bash

sudo cp -r ./* /etc/nixos/
```
2. Rebuild your NixOS configuration:

```bash

    sudo nixos-rebuild switch
```
## Configuration

This repository includes configurations for:

    - System packages
    - User environments
    - Services (e.g., SSH, Oh My Zsh)
    - Custom scripts

### Key Configuration Files

    `configuration.nix`: Main system configuration.
    `hardware-configuration.nix`: Hardware-specific settings.
    `additional-packages.nix`: Additional packages I use.
    `services.nix`: Custom service configurations.

## Usage

After applying the configurations, you can use NixOS as usual. Any customizations I've made will be reflected in your environment.

## Customization

You can modify the configuration files as per your needs. Here are some common modifications:

    - Add or remove packages in environment.systemPackages.
    - Modify user settings in users.users.yourusername.
    - Configure services in services.nix.