# Pterodactyl Panel Update Script

A small bash script that updates an existing Pterodactyl Panel installation to the latest release.  
It follows the official update process and automates all steps, making updates quicker and reducing mistakes.

This project is not associated with the official Pterodactyl team.

---

## One-line update command

```bash
bash <(curl -sSL https://isthisvishal.github.io/Pterodactyl-Panel-Update-Rebuild-/pterodactyl.update)
```

---

## Supported operating systems

This script supports Debian-based servers commonly used for Pterodactyl.

### Supported panel update environments

| Operating System | Version | Supported | PHP Version |
| ---------------- | ------- | --------- | ----------- |
| Ubuntu           | 20.04   | ✔️ Yes    | 8.1+        |
|                  | 22.04   | ✔️ Yes    | 8.1+        |
|                  | 24.04   | ✔️ Yes    | 8.1+        |
| Debian           | 10      | ✔️ Yes    | 8.1+        |
|                  | 11      | ✔️ Yes    | 8.1+        |
|                  | 12      | ✔️ Yes    | 8.1+        |

---

## Requirements

- Root or sudo access  
- PHP 8.1 or newer  
- Composer installed  
- MySQL or MariaDB  
- Nginx or Apache  
- Panel installed at:

```
/var/www/pterodactyl
```

---

## Manual usage

```bash
curl -O https://isthisvishal.github.io/Pterodactyl-Panel-Update-Rebuild-/pterodactyl.update
chmod +x pterodactyl.update
./pterodactyl.update
```

---

## What the script does

1. Enables maintenance mode  
2. Downloads the latest panel release  
3. Extracts updated files  
4. Installs Composer dependencies  
5. Runs database migrations  
6. Clears cached files  
7. Fixes permissions  
8. Disables maintenance mode  

---

## Notes

- Always back up before updating  
- This updates **Panel only**, not Wings  
- Wings updates must be done separately  

---

## License

MIT License  
© 2025 Vishal GG
