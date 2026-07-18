# Linux User and Group Management

## Overview

Linux is a multi-user operating system. Each user has specific permissions and belongs to one or more groups.

---

## Display Current User

```bash
whoami
```

Shows the username of the current logged-in user.

---

## Display User Information

```bash
id
```

Example:

```text
uid=1000(krupa) gid=1000(krupa) groups=1000(krupa),27(sudo)
```

---

## Display Logged-in Users

```bash
who
```

Shows all currently logged-in users.

---

## Create a New User

```bash
sudo useradd username
```

Example:

```bash
sudo useradd john
```

---

## Set User Password

```bash
sudo passwd john
```

---

## Delete a User

```bash
sudo userdel john
```

Delete user and home directory:

```bash
sudo userdel -r john
```

---

## Create a New Group

```bash
sudo groupadd developers
```

---

## Add User to a Group

```bash
sudo usermod -aG developers john
```

---

## Remove User from a Group

```bash
sudo gpasswd -d john developers
```

---

## Display Group Information

```bash
groups
```

or

```bash
groups username
```

---

## Switch User

```bash
su username
```

Example:

```bash
su john
```

---

## Run Commands as Administrator

```bash
sudo command
```

Example:

```bash
sudo apt update
```

---

# Common Commands

| Command - Purpose |

| whoami - Show current user |
| id - Show user ID and groups |
| who - Show logged-in users |
| useradd - Create a user |
| userdel - Delete a user |
| passwd - Set password |
| groupadd - Create a group |
| usermod - Modify user |
| groups - Show user groups |
| sudo - Run command as administrator |

---

# What I Learned

- Linux supports multiple users.
- Every user belongs to one or more groups.
- Groups simplify permission management.
- `sudo` allows authorized users to execute administrative commands.
- `id`, `whoami`, and `groups` help inspect user information.
