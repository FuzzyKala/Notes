1.  It's supposed to turn on SMB server function on router's GUI or use following command .\
    *Go to /etc to find out **smb.conf**\
    *`[Windows]\
      path = /media/Windows\
      guest ok = yes\
      writeable = yes`
    *Go to /media/Windows/sharefoldername or /home/username/share depending on your devices.

2.  
