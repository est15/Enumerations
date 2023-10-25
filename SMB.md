# SMB Enumeration 

### SMBClient
List SMB Shares
```bash
smbclient -L \\\\<ip>\\ -U <guest/user>
```

Connect to SMB Share
```bash
smbclient \\\\<ip>\\<share> -U <guest/user>
```
### SMBMap
List the shares and permissions
```bash
smbmap -u <user> -p <pass> -H <ip>
```


### CrackMapExec SMB Enumeration
Enumerate users by Bruteforcing RIDs
```bash
crackmapexec smb <ip> -u <user> -p <pass> --rid-brute
```
