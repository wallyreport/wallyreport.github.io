# using lftp to mirror a remote directory to a local directory

```bash
lftp server.com -u username,pass -e 'glob -d mirror Documents --use-pget-n=16 && exit'
```

    % lftp -e 'mirror <remote download dir> <local download dir>' -u <username>,<pass> -p <port> <hostname>

http://www.russbrooks.com/2010/11/19/lftp-cheetsheet
