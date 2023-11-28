1.  It's supposed to turn on SMB server function on router's GUI or use following command .\
    *Go to /etc to find out **smb.conf**
    *`[Windows]                                
      comment = CT1000MX 500SSD1's Windows                                  
      path = /media/Windows        
      guest ok = yes                      
      writeable = yes                                                       
      directory mode = 0777        
      create mask = 0777                  
      map archive = no                                                      
      map hidden = no              
      map read only = no                  
      map system = no                                                       
      store dos attributes = yes`
    *Go to /media/Windows/sharefoldername or /home/username/share depending on your devices.

2.  
