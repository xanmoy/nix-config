# NixOs Commands


## Edit Your Configuration File:
`sudo nano /etc/nixos/configuration.nix`

## Add the Package:
`environment.systemPackages = with pkgs; [
  packageName
];`

## Rebuild Your System: 
`sudo nixos-rebuild switch`

## Managing Git:
`cp /etc/nixos/hardware-configuration.nix ~/nixos-config/`
`cp /etc/nixos/configuration.nix ~/nixos-config/`

## Update Nix Channels:
`sudo nix-channel --update`

## Upgrade the System: 
`sudo nixos-rebuild switch --upgrade`

## Rebuild the System (Optional): 
`sudo nixos-rebuild switch`

## Clean Up Old Generations (Optional): 
`sudo nix-collect-garbage`


**If you want to install a package for immediate use without modifying your configuration, you can use nix-shell:**

## Install a Package Temporarily:
`nix-shell -p packageName`


**The nix-env command is a tool used to manage packages in Nix. It allows you to install, upgrade, remove, and query user-specific packages without affecting the system-wide configuration. Here’s a quick overview of how to use nix-env:**

## Install a Package:
`nix-env -i packageName`

## List Installed Packages:
`nix-env -q`

## Upgrade a Package:
`nix-env -u packageName`

## To upgrade all installed packages:
`nix-env -u`

## Remove a Package:
`nix-env -e packageName`

## Search for Packages:
`nix-env -qaP searchTerm`

## Rollback:
`nix-env --rollback`

