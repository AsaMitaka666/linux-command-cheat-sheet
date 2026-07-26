# Linux Security Hardening

Security hardening is the process of improving a Linux system's security by reducing risks and preventing unauthorized access.

---

# System Updates

## Description

Keeping packages updated helps fix security vulnerabilities.

## Commands

Update package lists:

```bash
sudo apt update
```

Upgrade installed packages:

```bash
sudo apt upgrade
```

---

# Strong Passwords

## Description

Strong passwords help protect user accounts.

Check password policy:

```bash
sudo nano /etc/login.defs
```

---

# sudo Security

## Description

`sudo` allows users to execute commands with administrator privileges.

Edit sudo configuration:

```bash
sudo visudo
```

---

# SSH Security

## Description

SSH should be configured securely to reduce unauthorized access.

Edit SSH configuration:

```bash
sudo nano /etc/ssh/sshd_config
```

Important settings:

Disable root login:

```text
PermitRootLogin no
```

Change default SSH port:

```text
Port 2222
```

Restart SSH:

```bash
sudo systemctl restart ssh
```

---

# Disable Unused Services

## Description

Removing unnecessary services reduces attack surface.

List services:

```bash
systemctl list-units --type=service
```

Stop a service:

```bash
sudo systemctl stop service_name
```

Disable service:

```bash
sudo systemctl disable service_name
```

---

# Fail2ban

## Description

Fail2ban protects services against brute-force attacks.

Install:

```bash
sudo apt install fail2ban
```

Check status:

```bash
sudo systemctl status fail2ban
```

---

# File Permissions

## Description

Correct permissions prevent unauthorized access.

Check permissions:

```bash
ls -l
```

Change permissions:

```bash
chmod 600 file
```

Change ownership:

```bash
chown user:group file
```

---

# Security Checklist

- Keep system updated
- Use strong passwords
- Disable root SSH login
- Use firewall rules
- Remove unused services
- Monitor system logs
