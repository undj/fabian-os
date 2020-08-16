# debian-live-build-fabian

Debian LiveCD with custom software and logos from Fabian and installer 

## To speedup mirrors use

LB_MIRROR_BOOTSTRAP="http://deb.debian.org/debian/"
LB_MIRROR_CHROOT_BACKPORTS="http://deb.debian.org/debian/"

## Build

cd livecd-custom

### Create chroot

lb config

### Clean and build

sudo lb clean; sudo lb build

scripts on chroot:

    config/hooks/live/0100-workbench.hook.chroot

Package lists:

    config/package-lists/

livecd config:
    auto/config
