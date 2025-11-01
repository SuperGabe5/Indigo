# CeriumOS &nbsp; [![bluebuild build badge](https://github.com/blue-build/template/actions/workflows/build.yml/badge.svg)](https://github.com/blue-build/template/actions/workflows/build.yml)

This is my solution to fill in the gap that may be left by the death of ChromiumOS

It is now also my Flagship System as of CeriumOS 43 (aka the NewUI Update)
## Installation

> [!WARNING]  
> THIS IS A BETA VERSION OF THE NewUI UPDATE, IT IS BASED ON FEDORA KINOITE 43
> **You may need to perform a clean install of this system for this Update if it can't rebase correctly**
> this is due to major stack overhauls and other overhauls

> [Note:]
> For new users the install process is simlar to the Old UI but it does inherit the changes to anaconda (and thus has Anaconda-WebUI) from upstream fedora

To rebase an existing atomic Fedora installation to the latest build:

- First rebase to the unsigned image, to get the proper signing keys and policies installed:
  ```
  rpm-ostree rebase ostree-unverified-registry:ghcr.io/supergabe5/cerium:latest
  ```
- Reboot to complete the rebase:
  ```
  systemctl reboot
  ```
- You Can migrate from any rpm-ostree based system, like so:
  ```
  rpm-ostree rebase -r ostree-image-signed:docker://ghcr.io/supergabe5/cerium:latest
  ```

The `latest` tag will automatically point to the latest build. That build will still always use the Fedora version specified in `recipe.yml`, so you won't get accidentally updated to the next major version.

## ISO
Coming Soon

## Verification

These images are signed with [Sigstore](https://www.sigstore.dev/)'s [cosign](https://github.com/sigstore/cosign). You can verify the signature by downloading the `cosign.pub` file from this repo and running the following command:

```bash
cosign verify --key cosign.pub ghcr.io/supergabe5/cerium
```
