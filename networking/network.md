# Linux Network Commands

Linux provides powerful tools for checking network connections, interfaces, and troubleshooting network problems.

---

# ip

## Description

`ip` is the modern command for managing and viewing network interfaces.

## Syntax

```bash
ip command
```

## Show network interfaces

```bash
ip addr
```

## Show routing table

```bash
ip route
```

---

# ping

## Description

`ping` checks connectivity between your computer and another host.

## Syntax

```bash
ping hostname
```

## Example

```bash
ping google.com
```

---

# ss

## Description

`ss` displays socket and network connection information.

## Syntax

```bash
ss
```

## Show listening ports

```bash
ss -tuln
```

---

# netstat

## Description

`netstat` displays network connections and statistics.

## Example

```bash
netstat -tulnp
```

Note: `ss` is the modern replacement for `netstat`.

---

# nslookup

## Description

`nslookup` queries DNS information.

## Example

```bash
nslookup google.com
```

---

# dig

## Description

`dig` performs detailed DNS queries.

## Example

```bash
dig google.com
```

---

# traceroute

## Description

`traceroute` shows the path packets take to reach a destination.

## Example

```bash
traceroute google.com
```

---

# hostname

## Description

`hostname` displays or changes the system hostname.

## Example

```bash
hostname
```
