## Exagear Desktop ARM64

#### About:
![intro](https://cdn.discordapp.com/attachments/763587003672428575/803231537809850458/IMG_20210125_172452.png)

ExaGear Desktop is a virtual machine that implements a virtual x86 Linux container on ARM-based mini PCs, enabling the direct and simultaneous running of both x86 Linux and native applications.

But it's discontinued, so this is it's package with key and how to fix it's apt error and some other stuff


#### Installation:-

Alternately, you can also use this video tutorial:-
https://youtu.be/ll6sPtcWDtI
(Note: this is installation of exagear desktop for arm64 on Debian proot.)

(1)To install patch, first clone it to pc:-
``` git clone https://github.com/SamarJi/Fixed-image-for-Exagear-Desktop ```

(2) Once cloned , if you got some errors while using apt update,use these commands :-
``` apt remove apt ```

That apt have bug, which cannot take updates
Install packages from cloned repository inside exagear, these were fixed apt files for exagear that can give updates
(3) Replace exagear's sources.list which is located in `/opt/exagear/images/debian-9/etc/apt/sources.list` with this repository's `sources.list`
 
(4) Once all done, you can use `apt update` can will got latest updates, don't use apt `upgrade`

# Current Updates:-

(1) Currently, it tested on ubuntu and debian proot inside termux and in linux deploy.

(2) Wine works which installed from default repository of exagear for wine.

(3) Python3 won't install in exagear.
