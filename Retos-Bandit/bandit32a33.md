# Bandit

## Objetivo
Después de todo esto `git`, es hora de otro escape. ¡Buena suerte!
## Datos de acceso
Usuario: bandit32
Password: rmCBvG56y58BXzv98yZGdO7ATVL5dW8y
## Solucion
```shell
Welcome to OverTheWire!
If you find any problems, please report them to the #wargames channel on
discord or IRC.
--[ Playing the games ]--
  This machine might hold several wargames.
  If you are playing "somegame", then:
    * USERNAMES are somegame0, somegame1, ...
    * Most LEVELS are stored in /somegame/.
    * PASSWORDS for each level are stored in /etc/somegame_pass/.
  Write-access to homedirectories is disabled. It is advised to create a
  working directory with a hard-to-guess name in /tmp/.  You can use the
  command "mktemp -d" in order to generate a random and hard to guess
  directory in /tmp/.  Read-access to both /tmp/ is disabled and to /proc
  restricted so that users cannot snoop on eachother. Files and directories
  with easily guessable or short names will be periodically deleted! The /tmp
  directory is regularly wiped.
  Please play nice:
    * don't leave orphan processes running
    * don't leave exploit-files laying around
    * don't annoy other players
    * don't post passwords or spoilers
    * again, DONT POST SPOILERS!
      This includes writeups of your solution on your blog or website!
--[ Tips ]--
  This machine has a 64bit processor and many security-features enabled
  by default, although ASLR has been switched off.  The following
  compiler flags might be interesting:
    -m32                    compile for 32bit
    -fno-stack-protector    disable ProPolice
    -Wl,-z,norelro          disable relro
  In addition, the execstack tool can be used to flag the stack as
  executable on ELF binaries.
  Finally, network-access is limited for most levels by a local
  firewall.
--[ Tools ]--
 For your convenience we have installed a few useful tools which you can find
 in the following locations:
    * gef (https://github.com/hugsy/gef) in /opt/gef/
    * pwndbg (https://github.com/pwndbg/pwndbg) in /opt/pwndbg/
    * peda (https://github.com/longld/peda.git) in /opt/peda/
    * gdbinit (https://github.com/gdbinit/Gdbinit) in /opt/gdbinit/
    * pwntools (https://github.com/Gallopsled/pwntools)
    * radare2 (http://www.radare.org/)
 Both python2 and python3 are installed.
--[ More information ]--
  For more information regarding individual wargames, visit
  http://www.overthewire.org/wargames/
  For support, questions or comments, contact us on discord or IRC.
  Enjoy your stay!
WELCOME TO THE UPPERCASE SHELL
//Importante
>> ls
sh: 1: LS: not found
>> man
sh: 1: MAN: not found
//usamos el comando $0 para entrar al shell
>> $0
$ ls -la
total 36
drwxr-xr-x  2 root     root      4096 Sep  1 06:30 .
drwxr-xr-x 49 root     root      4096 Sep  1 06:30 ..
-rw-r--r--  1 root     root       220 Jan  6  2022 .bash_logout
-rw-r--r--  1 root     root      3771 Jan  6  2022 .bashrc
-rw-r--r--  1 root     root       807 Jan  6  2022 .profile
-rwsr-x---  1 bandit33 bandit32 15124 Sep  1 06:30 uppershell
$ whoami
bandit33
$ cat /etc/bandit_pass/bandit33
odHo63fHiFqcWWJG9rLiLDtPm45KzUKy
$ exit
>> ^CConnection to bandit.labs.overthewire.org closed.
```
## Notas adicionales
Con $0 podemos entrar en un shell para salir de donde estabamos Solo como recordatorio recuerda que el comando whoami te dice el usuario con el que estas conectado.
## Referencias

