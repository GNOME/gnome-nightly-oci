# Container images with the GNOME nightly runtime

This repo contains the docker files used to build the container images that are used
to build Flatpak packages in the gtilab-CI.

The base image contains `flatpak`, `flatpak-builder` along with all their dependancies.
It also contains `git` and `xvfb` since they are quite common packages and used in the CI
config of most GNOME apps.

It's possible to add images with various sdk bundles too. Currenlty there is only the `rust-bundle`
image which uses the `nightly:master` fot it's base and also contains the [FreeDesktop Rust Sdk Extensions][rust].

## Adding more sdk-bundles

TBA


[rust]: https://github.com/flathub/org.freedesktop.Sdk.Extension.rust-stable
