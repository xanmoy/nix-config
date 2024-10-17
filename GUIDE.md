# NixOs Commands


## Edit Your Configuration File:
```bash
sudo nano /etc/nixos/configuration.nix
```

## Add the Package:
```bash
environment.systemPackages = with pkgs; [
  packageName
]; 
```

## Rebuild Your System: 
```bash
sudo nixos-rebuild switch
```

## Managing Git:
```bash
cp /etc/nixos/hardware-configuration.nix ~/nixos-config/
```
```bash
cp /etc/nixos/configuration.nix ~/nixos-config/
```

## Update Nix Channels:
```bash
sudo nix-channel --update
```

## Upgrade the System: 
```bash
sudo nixos-rebuild switch --upgrade
```

## Rebuild the System (Optional): 
```bash
sudo nixos-rebuild switch
```

## Clean Up Old Generations (Optional): 
```bash
sudo nix-collect-garbage
```


**If you want to install a package for immediate use without modifying your configuration, you can use nix-shell:**

## Install a Package Temporarily:
```bash
nix-shell -p packageName
```


**The nix-env command is a tool used to manage packages in Nix. It allows you to install, upgrade, remove, and query user-specific packages without affecting the system-wide configuration. Here’s a quick overview of how to use nix-env:**

## Install a Package:
```bash
nix-env -i packageName
```

## List Installed Packages:
```bash
nix-env -q
```

## Upgrade a Package:
```bash
nix-env -u packageName
```

## To upgrade all installed packages:
```bash
nix-env -u
```

## Remove a Package:
```bash
nix-env -e packageName
```

## Search for Packages:
```bash
nix-env -qaP searchTerm
```

## Rollback:
```bash
nix-env --rollback
```

