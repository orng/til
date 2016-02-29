#Automatically reconfigure the chosen nameserver
So I just set up a new router and while I was able to connect to the router just fine and access the admin panel I seemed unable to connect to any webpages. However, all other devices at home were able to connect to the internet just fine. After some digging around it turned out that /etc/resolve.conf still reffered to the address of the previous router and thus the setup for the nameserver was incorrect. To remedy this all I had to do was to run:

```
sudo dhclient
```

dhclient took care of automatically configuring the nameserver stuff for me.
