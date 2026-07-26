# Linux User Management Commands

Linux is a multi-user operating system. User management is an important part of system administration and security.

---

# whoami

## Description

`whoami` displays the current logged-in user.

## Syntax

```bash
whoami
```

---

# id

## Description

`id` shows user identity information including UID and groups.

## Syntax

```bash
id
```

---

# who

## Description

`who` shows users currently logged into the system.

## Syntax

```bash
who
```

---

# w

## Description

`w` displays logged-in users and their activity.

## Syntax

```bash
w
```

---

# groups

## Description

`groups` shows groups that a user belongs to.

## Syntax

```bash
groups
```

---

# useradd

## Description

`useradd` creates a new user.

## Syntax

```bash
sudo useradd username
```

## Example

```bash
sudo useradd asa
```

---

# passwd

## Description

`passwd` changes a user's password.

## Syntax

```bash
sudo passwd username
```

## Example

```bash
sudo passwd asa
```

---

# usermod

## Description

`usermod` modifies user accounts.

## Example

Add user to a group:

```bash
sudo usermod -aG group username
```

---

# userdel

## Description

`userdel` removes a user account.

## Syntax

```bash
sudo userdel username
```
