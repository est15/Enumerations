# Forensics CLI & GUI Tools to Keep in Mind

## [Oletools](https://github.com/decalage2/oletools)
Python package of tools to analyze OLE and Microsoft Office Documents.

## [Volatility](https://github.com/volatilityfoundation/volatility)
### Get Memory Dump Profile
```bash
python vol.py -f <memdump.elf> imageinfo
```
### Examine Processes Running
```bash 
python vol.py -f <memdump.elf> --profile=<profile_from_above> pstree
```
