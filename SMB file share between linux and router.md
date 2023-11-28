1.  It's supposed to turn on SMB server function on router's GUI or follow the step below.\
    *   Go to /etc to find out **smb.conf** \
    *   <pre>
          <p>[Windows]                                
               comment = CT1000MX 500SSD1's Windows                                  
               path = /media/Windows        
               guest ok = yes                      
               writeable = yes                                                       
  
           </p>
      </pre>
    *   Go to /media/Windows/sharefoldername or /home/username/share depending on your devices.

2.  
