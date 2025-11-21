# Indigo Linux &nbsp; [![bluebuild build badge](https://github.com/blue-build/template/actions/workflows/build.yml/badge.svg)](https://github.com/blue-build/template/actions/workflows/build.yml)

Welcome to the Indigo Linux System Repo

Indigo Linux is a family of immutable Fedora-based Systems

There are a few flavors to choose from:

1. KDE, the flagship one (called by the former CeriumOS name "cerium")

2. MATE, The Classic One ("verde")

3. LXQt, Home Server ("server")

   (more flavors coming soon)
   
## Installation

I do not reccomend that you rebase from one atomic fedora system to another as it has caused problems in my testing

So if you want to install Indigo Linux you must do a clean install

The `latest` tag will automatically point to the latest build. That build will still always use the Fedora version specified in `recipe.yml`, so you won't get accidentally updated to the next major version.

## ISO Files
Coming Soon

## Verification

These images are signed with [Sigstore](https://www.sigstore.dev/)'s [cosign](https://github.com/sigstore/cosign). You can verify the signature by downloading the `cosign.pub` file from this repo and running the following command:

```bash
cosign verify --key cosign.pub ghcr.io/supergabe5/cerium
```
