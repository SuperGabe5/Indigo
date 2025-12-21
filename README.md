# Indigo Linux

Welcome to the Old Indigo Linux System Repo

Indigo Linux was a family of immutable Fedora-based Systems

There were a few flavors to choose from:

1. KDE, the flagship one (called by the former CeriumOS name "cerium")

2. MATE, The Classic One ("verde")

3. LXQt, Home Server ("server")

4. Mint, Used Cinnamon Desktop Environment

   (more flavors were planned)
   
## Installation

This system has been cancelled due to a concestant RPM gpg error when trying to make an ISO file while the fedora version of the image is 43,

I am currently in the process of rebasing this system in the fallowing

MATE and Cinnamon:

Artix Linux (dinit with XLibre)

Home Server:

EndeavorOS (xfce4) with cockpit installed by default until my own solution is ready.

Other Information:

LXQt edition has been deprecated in this Rebase

KDE edition has been deprecated in this Rebase because KDE has officially removed x11 support.

I may or may not add it back in if KDE brings x11 support back with official XLibre being noted as officially supported by KDE.

I'm also Beginning to think about ditching Linux entirely as a base and going to BSD as upstream Linux has been making too many less than favorable changes recently 

(most condemning thing in my opinion: THE LITERAL CREATOR OF THE KERNEL HAS GONE TO FEDORA WITH GNOME AND WAYLAND)

## ISO Files
Canceled

## Verification

These images were signed with [Sigstore](https://www.sigstore.dev/)'s [cosign](https://github.com/sigstore/cosign). You can verify the signature by downloading the `cosign.pub` file from this repo and running the following command:

```bash
cosign verify --key cosign.pub ghcr.io/supergabe5/cerium
```
