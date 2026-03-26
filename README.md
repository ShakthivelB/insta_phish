# 🎣 Instagram Phishing Tool (Linux & Termux Compatible without root)

A phishing tool to simulate instagram credential harvesting for **educational and ethical hacking purposes**.

- 📡 Serves a fake email login page on `127.0.0.1:3333`
- 🌐 Uses **Cloudflare Tunnel** (`cloudflared`) to expose it publicly
- 📝 Captures credentials and saves them to `www/log.txt`

> ⚠️ **DISCLAIMER**  
> This tool is for authorized security testing and education purpose only.  
> Do **not** use it on real targets without **explicit written permission**.

---

---

## ⚙️ Requirements

- Termux or Linux (Ubuntu/Debian/Kali)
- `php`
- `cloudflared` (Cloudflare Tunnel)

---
```
apt update
apt install php
apt install cloudflared
```
## Start the tool 

`insga_phish.sh`
      or
`php -d opcache.enable=0 -S 127.0.0.1:3333 -t www`

## Cloudflare tunnel

`cloudflared tunnel --url http://127.0.0.1:3333`
