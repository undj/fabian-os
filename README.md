Guida operativa (README.md) :


    Generare l’ISO

1) Installazione di Debian 10 LXDE 64 bit su Virtualbox (almeno 20GB spazio)

2) Update e upgrade del sistema

3) Installare pacchetti consigliati
sudo apt-get install git  live-build debootstrap squashfs-tools xorriso isolinux syslinux-efi grub-pc-bin grub-efi-amd64-bin mtools

4) Scaricare il repository di Fabian da Github
'''git clone https://github.com/undj/fabian-os'''

5) Spostarsi nella cartella dove è possibile generare l’ISO
cd fabian-os/livecd-custom

6) Generare l’ISO (processo lungo)
lb build



    Testare l’ISO

Loggarsi tramite google e caricare l’iso nel drive commentanto il file di testo all’interno della cartella
https://drive.google.com/drive/folders/176z5kik3Aw9pAr5b0tlHoYxK1FMbgBw1?hl=i


    Documentazione estesa
https://drive.google.com/drive/folders/1ax7TDqJ8GT2HI5_2woL459u6kmdnajRr

