# To use this, you just need to add these.
### On flake.nix
in the inputs
```nix
  zen-browser.url = "github:444heaven/zen-browser-nixos-flake";
```
in the outputs you just need to add zen-browser
### On home.nix
in the imports
```nix
    inputs.zen-browser.homeManagerModules.zen-browser
```
then to you is, add also this on home.nix
```nix
    programs.zen-browser.enable = true;
```
