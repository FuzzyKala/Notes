1. make sure the SSH function is available and enabled on the remote device. \
   ![image](./images/1.png)

2. try to use ssh to log in (still need password), make sure you can log in properly, in my case:\
   `ssh admin@192.168.123.1`\
   ![image](./images/2.png)

3. generate the ssh-key by typing the command (I have no idea why my router only accepts ecdsa):\
   `ssh-keygen -t ecdsa`\
   ![image](./images/3.png)

4. exit to the local shell and type (it might need you to type the password in this step.):\
   `ssh-copy-id -i ~/.ssh/id_ecdsa.pub admin@192.168.123.1`\
   ![image](./images/4.png)

5. login without password\
   ![image](./images/5.png)
