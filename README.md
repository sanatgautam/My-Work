sanat@sanat-desktop:~$ ssh-keygen -t rsa -b 4096 -C "alive.for.reason@gmail.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/home/sanat/.ssh/id_rsa): 
Created directory '/home/sanat/.ssh'.
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/sanat/.ssh/id_rsa.
Your public key has been saved in /home/sanat/.ssh/id_rsa.pub.
The key fingerprint is:
00:1a:5e:7b:71:77:fe:ed:10:81:80:93:a9:2b:5e:4e alive.for.reason@gmail.com
The key's randomart image is:
+--[ RSA 4096]----+
|  . o . .+o....  |
| . + o o=. o.  . |
|  o . o. .  . .  |
|     ...     . o |
|       .S     o .|
|    . E        o |
|   . =          .|
|    . .          |
|                 |
+-----------------+
sanat@sanat-desktop:~$ eval "$(ssh-agent -s)"
Agent pid 2927
sanat@sanat-desktop:~$ ssh-add ~/.ssh/id_rsa
Identity added: /home/sanat/.ssh/id_rsa (/home/sanat/.ssh/id_rsa)
sanat@sanat-desktop:~$ sudo apt-get install xclip
sudo: /var/lib/sudo/sanat writable by non-owner (040777), should be mode 0700
[sudo] password for sanat: 
sanat is not in the sudoers file.  This incident will be reported.
sanat@sanat-desktop:~$ su
Password: 
root@sanat-desktop:/home/sanat# sudo apt-get install xclip
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages were automatically installed and are no longer required:
  language-pack-kde-en language-pack-kde-en-base kde-l10n-engb
Use 'apt-get autoremove' to remove them.
The following NEW packages will be installed:
  xclip
0 upgraded, 1 newly installed, 0 to remove and 451 not upgraded.
Need to get 19.7 kB of archives.
After this operation, 94.2 kB of additional disk space will be used.
Get:1 http://in.archive.ubuntu.com/ubuntu/ precise/universe xclip i386 0.12-1 [19.7 kB]
Fetched 19.7 kB in 0s (21.4 kB/s)
Selecting previously unselected package xclip.
(Reading database ... 299519 files and directories currently installed.)
Unpacking xclip (from .../archives/xclip_0.12-1_i386.deb) ...
Processing triggers for man-db ...
Setting up xclip (0.12-1) ...
root@sanat-desktop:/home/sanat# su sanat
sanat@sanat-desktop:~$ xclip -sel clip < ~/.ssh/id_rsa.pub
sanat@sanat-desktop:~$ ssh -T git@github.com
The authenticity of host 'github.com (192.30.252.131)' can't be established.
RSA key fingerprint is 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.
Are you sure you want to continue connecting (yes/no)? yes
Warning: Permanently added 'github.com,192.30.252.131' (RSA) to the list of known hosts.
Hi sanatgautam! You've successfully authenticated, but GitHub does not provide shell access.
