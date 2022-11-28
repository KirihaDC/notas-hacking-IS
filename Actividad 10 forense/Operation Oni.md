# Objetivo
Descargue esta imagen de disco, busque la clave e inicie sesión en la máquina remota.Nota: si está utilizando webshell, descargue y extraiga la imagen del disco en `/tmp`su directorio de inicio.

# Solución 
┌──(kiriha㉿kali)-[~/Descargas]
└─$ gzip -d disk.img.gz 
                                                                                                                                                                                                                                            
┌──(kiriha㉿kali)-[~/Descargas]
└─$ mmls disk.img   
DOS Partition Table
Offset Sector: 0
Units are in 512-byte sectors

      Slot      Start        End          Length       Description
000:  Meta      0000000000   0000000000   0000000001   Primary Table (#0)
001:  -------   0000000000   0000002047   0000002048   Unallocated
002:  000:000   0000002048   0000206847   0000204800   Linux (0x83)
003:  000:001   0000206848   0000471039   0000264192   Linux (0x83)
                                                                                                                                                                                                                                            
┌──(kiriha㉿kali)-[~/Descargas]
└─$ fls -o 206848 disk.img 
d/d 458: home
d/d 11: lost+found
d/d 12: boot
d/d 13: etc
d/d 79: proc
d/d 80: dev
d/d 81: tmp
d/d 82: lib
d/d 85: var
d/d 94: usr
d/d 104: bin
d/d 118: sbin
d/d 464: media
d/d 468: mnt
d/d 469: opt
d/d 470: root
d/d 471: run
d/d 473: srv
d/d 474: sys
V/V 33049: $OrphanFiles
                                                                                                                                                                                                                                            
┌──(kiriha㉿kali)-[~/Descargas]
└─$ fls -o 206848 disk.img 470
r/r 2344: .ash_history
d/d 3916: .ssh
                                                                                                                                                                                                                                            
┌──(kiriha㉿kali)-[~/Descargas]
└─$ fls -o 206848 disk.img 3916
r/r 2345: id_ed25519
r/r 2346: id_ed25519.pub
                                                                                                                                                                                                                                            
┌──(kiriha㉿kali)-[~/Descargas]
└─$ icat -o 206848 disk.img 2345
-----BEGIN OPENSSH PRIVATE KEY-----
b3BlbnNzaC1rZXktdjEAAAAABG5vbmUAAAAEbm9uZQAAAAAAAAABAAAAMwAAAAtzc2gtZW
QyNTUxOQAAACBgrXe4bKNhOzkCLWOmk4zDMimW9RVZngX51Y8h3BmKLAAAAJgxpYKDMaWC
gwAAAAtzc2gtZWQyNTUxOQAAACBgrXe4bKNhOzkCLWOmk4zDMimW9RVZngX51Y8h3BmKLA
AAAECItu0F8DIjWxTp+KeMDvX1lQwYtUvP2SfSVOfMOChxYGCtd7hso2E7OQItY6aTjMMy
KZb1FVmeBfnVjyHcGYosAAAADnJvb3RAbG9jYWxob3N0AQIDBAUGBw==
-----END OPENSSH PRIVATE KEY-----
                                                                                                                                                                    
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ssh -i key_file -p 54701 ctf-player@saturn.picoctf.net
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@         WARNING: UNPROTECTED PRIVATE KEY FILE!          @
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
Permissions 0644 for 'key_file' are too open.
It is required that your private key files are NOT accessible by others.
This private key will be ignored.
Load key "key_file": bad permissions
ctf-player@saturn.picoctf.net's password: 
Permission denied, please try again.
ctf-player@saturn.picoctf.net's password: 
Permission denied, please try again.
ctf-player@saturn.picoctf.net's password: 
ctf-player@saturn.picoctf.net: Permission denied (publickey,password).
                                                                                                                                                                                                                                            
┌──(kiriha㉿kali)-[~/Descargas]
└─$ chmod 400 key_file
                                                                                                                                                                                                                                            
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ssh -i key_file -p 54701 ctf-player@saturn.picoctf.net
Welcome to Ubuntu 20.04.3 LTS (GNU/Linux 5.15.0-1023-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

This system has been minimized by removing packages and content that are
not required on a system that users do not log into.

To restore this content, you can run the 'unminimize' command.

The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

ctf-player@challenge:~$ ls
flag.txt
ctf-player@challenge:~$ cat 
.cache/   .ssh/     flag.txt  
ctf-player@challenge:~$ cat flag.txt 
picoCTF{k3y_5l3u7h_b5066e83}ctf-player@challenge:~$

# Notas adicionales 

# Referencias
