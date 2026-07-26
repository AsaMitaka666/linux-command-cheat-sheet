# Linux Process Commands

A process is a running instance of a program in Linux.

---

# ps

## Description

`ps` displays information about running processes.

## Syntax

```bash
ps
```

## Example

```bash
ps aux
```

---

# top

## Description

`top` provides a real-time view of running processes.

## Syntax

```bash
top
```

---

# htop

## Description

`htop` is an interactive process viewer.

## Install

```bash
sudo apt install htop
```

## Usage

```bash
htop
```

---

# kill

## Description

`kill` terminates a process using its PID.

## Syntax

```bash
kill PID
```

## Example

```bash
kill 1234
```

---

# pkill

## Description

`pkill` kills processes by name.

## Syntax

```bash
pkill process_name
```

## Example

```bash
pkill firefox
```

---

# systemctl

## Description

`systemctl` manages system services using systemd.

## Examples

Check service status:

```bash
systemctl status ssh
```

Start service:

```bash
systemctl start service_name
```

Stop service:

```bash
systemctl stop service_name
```

---

# journalctl

## Description

`journalctl` views system logs.

## Example

```bash
journalctl -xe
```
