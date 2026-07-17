# Linux File Permissions and Ownership

## Overview

Linux uses permissions to control who can read, write, or execute files and directories.

---

## Viewing Permissions

Use the `ls -l` command to view file permissions.

```bash
ls -l
```

Example output:

```text
-rwxr-xr-- 1 krupa users 1024 Jul 17 script.sh
```

The first 10 characters represent the file type and permissions.

---

## Permission Symbols

| Symbol | Meaning |
|--------|---------|
| r | Read |
| w | Write |
| x | Execute |

Permissions are assigned to:

- Owner
- Group
- Others

---

## Changing Permissions

### Numeric Method

```bash
chmod 755 script.sh
```

| Number | Permission |
|--------|------------|
| 7 | rwx |
| 6 | rw- |
| 5 | r-x |
| 4 | r-- |

Example:

```bash
chmod 644 notes.txt
chmod 755 backup.sh
```

---

### Symbolic Method

Add execute permission:

```bash
chmod +x script.sh
```

Remove write permission:

```bash
chmod -w file.txt
```

Grant read permission to others:

```bash
chmod o+r file.txt
```

---

## Changing Ownership

Use `chown` to change the owner of a file.

```bash
sudo chown username file.txt
```

Change owner and group:

```bash
sudo chown username:groupname file.txt
```

---

## Changing Group

```bash
sudo chgrp developers project.txt
```

---

## Useful Commands

```bash
ls -l
chmod
chown
chgrp
```

---

## What I Learned

- Linux permissions protect files from unauthorized access.
- `chmod` changes permissions.
- `chown` changes ownership.
- `chgrp` changes the group ownership.
- Numeric permissions are easier for assigning multiple permissions at once.
