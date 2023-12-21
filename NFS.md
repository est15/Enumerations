# TCP: 2049 - NFS Service Enumerations

## Nmap Enumeration Scripts
```bash
nmap -p2049 -sV --script=nfs-ls,nfs-showmount,nfs-statfs <host>
```

## View Mountable Folder
```bash
showmount -e <ip>
```

## Mount the Share 
```bash
mount -t nfs [-o vers=2] <ip>:<remote_folder> <local_folder> -o nolock
```
