i# SMB Enumeration 

## SMBClient
List SMB Shares
```bash
smbclient -L \\\\<ip>\\ -U <guest/user>
```

Connect to SMB Share
```bash
smbclient \\\\<ip>\\<share> -U <guest/user>
```
## SMBMap
List the shares and permissions
```bash
smbmap -u <user> -p <pass> -H <ip>
```


## CrackMapExec SMB Enumeration
Enumerate users by Bruteforcing RIDs
```bash
crackmapexec smb <ip> -u <user> -p <pass> --rid-brute
```

## RPCClient
Manually Enumerate RIDs
```bash
for i in $(seq 500 1100); do
    rpcclient -N -U "" 10.129.14.128 -c "queryuser 0x$(printf '%x\n' $i)" | grep "User Name\|user_rid\|group_rid" && echo "";
done
```

## Enum4Linux-ng
SMB Enumeration Scan:
```bash
./enum4linux-ng.py -A <ip> -oA <output>
```
