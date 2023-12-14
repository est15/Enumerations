# Bruteforcing HTTP(S) 

## Hydra
### HTTP-POST-FORM
```bash
hydra <IP or DOMAIN> -l user -P /usr/share/wordlists/rockyou.txt https-post-form "/path/for/login:Parameters=^USER^&Parameter=^PASS^:Error Text"
```
