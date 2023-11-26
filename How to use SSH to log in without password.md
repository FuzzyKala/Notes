1. make sure the SSH function is available and enabled on the remote device. \
   ![image](./images/1.png)

2. try to use ssh to log in (still need password), make sure you can log in properly, in my case:\
   `kala@G614JV:~$ ssh admin@192.168.123.1`\
   
   `BusyBox v1.29.3 (2022-01-02 20:45:37 CST) built-in shell (ash)`\
   `Enter 'help' for a list of built-in commands.`\
   `[RT-N56UB1-newif3D2-512M 3.4.3.9-099_22-01-3]# 2023-11-26 16:58:34`\
   `[RT-N56U_B1 /home/root]#`


4. generate the ssh-key by typing the command (I have no idea why my router only accepts ecdsa):\
   >```kala@G614JV:~$ ssh-keygen -t ecdsa```
   Generating public/private ecdsa key pair.
   Enter file in which to save the key (/home/kala/.ssh/id_ecdsa): 
   /home/kala/.ssh/id_ecdsa already exists.
   Overwrite (y/n)? y
   Enter passphrase (empty for no passphrase): 
   Enter same passphrase again: 
   Your identification has been saved in /home/kala/.ssh/id_ecdsa
   Your public key has been saved in /home/kala/.ssh/id_ecdsa.pub
   The key fingerprint is:
   SHA256:mQ+PaZ23WxhZvxWLdcF2K6xLVVaCxIaguV+T3+146Go kala@G614JV
   The key's randomart image is:
   +---[ECDSA 256]---+
   |        .. +..o.o|
   |       o  . +  *o|
   |      o    .. =o+|
   |       . o . *oo+|
   |      . S + =...o|
   |       . O * + .o|
   |        = * = oo.|
   |       .   oEo.o.|
   |           .++o..|
   +----[SHA256]-----+```


6. exit to the local shell and type (it might need you to type the password in this step.):\
   `ssh-copy-id -i ~/.ssh/id_ecdsa.pub admin@192.168.123.1`\
   ![image](./images/4.png)

7. login without password\
   ![image](./images/5.png)
