#   Router/Server side
It's supposed to turn on the SMB server function on the router's GUI or follow the steps below.\
    *   Go to /etc to find out **smb.conf** \
    *   add the configuration at the bottom of the configuration file.
        ```
        [Windows]
        path = /media/Windows
        guest ok = yes
        writeable = yes
        ```
    *   Go to /media/Windows/sharefoldername or /home/username/share depending on your devices.

#   Laptop/Client Side
open folder and use **connect to the server** then type the path, in my case "smb://192.168.123.1/".
after that, you should be able to see the folder called 'Windows/share' or whatever you named before.
