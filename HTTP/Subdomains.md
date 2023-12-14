# Subdomain Enumeration

## wFuzz
```bash
wfuzz -w /path/to/wordlist -H "Host: FUZZ.host.com"  host.com
```
Make sure to filter out responses based on code/lines/words/chars

## Gobuster Vhost
```bash
gobuster vhost --url https://example.com --wordlist /usr/share/SecLists/Discovery/DNS/subdomains-top1million-110000.txt --no-tls-validation --exclude-length <length>
```
Utilize gobuster when bruteforcing HTTPS subdomains
