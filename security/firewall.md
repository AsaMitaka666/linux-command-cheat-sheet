# Linux Firewall Commands

A firewall controls incoming and outgoing network traffic to improve system security.

---

# UFW

## Description

`ufw` (Uncomplicated Firewall) is a simple firewall management tool for Linux systems.

---

# ufw status

## Description

Shows the current firewall status.

## Syntax

```bash
sudo ufw status
```

---

# ufw enable

## Description

Enables the firewall.

## Example

```bash
sudo ufw enable
```

---

# ufw disable

## Description

Disables the firewall.

## Example

```bash
sudo ufw disable
```

---

# ufw allow

## Description

Allows specific connections.

## Example

Allow SSH:

```bash
sudo ufw allow ssh
```

Allow a port:

```bash
sudo ufw allow 80
```

---

# ufw deny

## Description

Blocks specific connections.

## Example

```bash
sudo ufw deny 23
```

---

# ufw delete

## Description

Removes firewall rules.

## Example

```bash
sudo ufw delete allow 80
```

---

# iptables

## Description

`iptables` is a powerful tool for managing Linux firewall rules.

## List rules

```bash
sudo iptables -L
```

## Example

Block an IP:

```bash
sudo iptables -A INPUT -s IP_ADDRESS -j DROP
```
