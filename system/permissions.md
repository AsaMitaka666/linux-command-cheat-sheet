# Linux File Permissions

Linux uses a permission system to control who can read, write, and execute files.

---

# ls -l

## Description

`ls -l` displays detailed information about files including permissions, owner, and group.

## Syntax

```bash
ls -l
```

## Example

```bash
ls -l file.txt
```

Example output:

```bash
-rwxr-xr-- 1 asa users 1024 file.txt
```

Permission format:

```text
rwx r-x r--
│   │   │
│   │   └── Others
│   └────── Group
└────────── Owner
```

---

# chmod

## Description

`chmod` changes file permissions.

## Syntax

```bash
chmod permissions filename
```

## Examples

Give execute permission:

```bash
chmod +x script.sh
```

Set permissions using numbers:

```bash
chmod 755 script.sh
```

Common permissions:

```text
755
Owner  : rwx
Group  : r-x
Others : r-x
```

```text
644
Owner  : rw-
Group  : r--
Others : r--
```

---

# chown

## Description

`chown` changes file ownership.

## Syntax

```bash
chown user filename
```

## Example

```bash
sudo chown asa file.txt
```

Change owner and group:

```bash
sudo chown asa:users file.txt
```

---

# chgrp

## Description

`chgrp` changes the group ownership of a file.

## Syntax

```bash
chgrp group filename
```

## Example

```bash
sudo chgrp developers project.txt
```

---

# umask

## Description

`umask` controls default permissions for newly created files.

## Syntax

```bash
umask
```

## Example

```bash
umask 022
```

---

# sudo

## Description

`sudo` allows users to run commands with administrator privileges.

## Example

```bash
sudo apt update
```
