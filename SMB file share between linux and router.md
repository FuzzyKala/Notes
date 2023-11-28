1.  It's supposed to turn on the SMB server function on the router's GUI or follow the steps below.\
    *   Go to /etc to find out **smb.conf** \
    *   ```
               [Windows]
               comment = CT1000MX 500SSD1's Windows                                  
               path = /media/Windows        
               guest ok = yes                      
               writeable = yes

    *   Go to /media/Windows/sharefoldername or /home/username/share depending on your devices.

2.  
