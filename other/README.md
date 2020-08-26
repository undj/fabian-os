<<<<<<< HEAD
# fabian-os


# Installazione di Debian 10 LXDE 64 bit su VirtualBox

### OPEN A TERMINAL ###

username:   fabian
password:   fabian
root pass:  fabian

# Aggiungere utente al gruppo sudo (logout and login required)
adduser fabian -G sudo

# Installare pacchetti
sudo apt-get install vlc blender thunderbird arduino fritzing evince gimp rsync git

# Aggiornare pacchetti
sudo apt-get update && apt-get upgrade

# GitHub clonare directory con personalizzazioni Fabian
sudo git clone https://github.com/undj/fabian-os

# Sostituire i file del sistema con le personalizzazioni scaricate e rimuovere il file scaricato
sudo rsync -avr fabian-os/usr/ usr/ && sudo rm -r fabian-os

# Configurare pacchetti non-free
> https://wiki.debian.org/it/SourcesList#formato_di_sources.list

# Change grub image
> https://wiki.debian.org/Grub2

# Change plymouth
> https://wiki.debian.org/it/plymouth
=======
# debian-live-build-fabian

Debian LiveCD with custom software and logos from Fabian and installer 

https://www.bustawin.com/create-a-custom-live-debian-9-the-pro-way/

http://nerotux.tuxfamily.org/index.php/Articles/DebianLiveHowto


## Requested packages

    apt install live-build debootstrap squashfs-tools xorriso isolinux syslinux-efi grub-pc-bin grub-efi-amd64-bin mtools

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
>>>>>>> other/master
