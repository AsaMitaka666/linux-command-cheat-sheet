# Linux SSH Commands

SSH (Secure Shell) is a protocol used to securely connect to remote Linux systems.

---

# ssh

## Description

`ssh` allows you to connect to another computer remotely.

## Syntax

```bash
ssh username@hostname
```

## Example

```bash
ssh asa@192.168.1.10
```

---

# scp

## Description

`scp` securely copies files between computers using SSH.

## Syntax

```bash
scp source destination
```

## Upload file to remote server

```bash
scp file.txt user@server:/home/user/
```

## Download file from remote server

```bash
scp user@server:/home/user/file.txt .
```

---

# ssh-keygen

## Description

`ssh-keygen` creates SSH authentication keys.

## Syntax

```bash
ssh-keygen
```

## Example

```bash
ssh-keygen -t rsa
```

---

# ssh-copy-id

## Description

`ssh-copy-id` copies your public key to a remote server.

## Syntax

```bash
ssh-copy-id username@hostname
```

## Example

```bash
ssh-copy-id asa@192.168.1.10
```

---

# SSH Config

## Description

SSH configuration allows you to create shortcuts for remote connections.

## Location

```bash
~/.ssh/config
```

## Example

```text
Host server
    HostName 192.168.1.10
    User asa
```

Connect:

```bash
ssh server
```
