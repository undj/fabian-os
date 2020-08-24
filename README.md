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
