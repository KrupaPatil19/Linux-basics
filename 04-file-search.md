# Linux File Search and Command Location

## Overview

Linux provides several commands to search for files, directories, and executable programs.

---

## find

The `find` command searches for files and directories.

### Syntax

```bash
find [path] [options] [expression]
```

### Examples

Find a file by name:

```bash
find . -name "notes.txt"
```

Find all shell scripts:

```bash
find . -name "*.sh"
```

Find directories:

```bash
find . -type d
```

Find files larger than 10 MB:

```bash
find . -size +10M
```

---

## locate

Searches for files using a pre-built database.

```bash
locate notes.txt
```

Update the database:

```bash
sudo updatedb
```

---

## which

Shows the location of an executable command.

```bash
which python
which git
which ls
```

Example output:

```text
/usr/bin/python
```

---

## whereis

Shows the executable, source code, and manual page locations.

```bash
whereis python
```

Example:

```text
python: /usr/bin/python /usr/share/man/man1/python.1.gz
```

---

## grep

Searches for text inside files.

Search for the word "error":

```bash
grep "error" log.txt
```

Ignore case:

```bash
grep -i "linux" notes.txt
```

Search recursively:

```bash
grep -r "main" .
```

Show line numbers:

```bash
grep -n "hello" file.txt
```

---

## Useful Commands

| Command | Purpose |
|---------|---------|
| find | Search files and directories |
| locate | Search using database |
| which | Locate executable |
| whereis | Locate executable, source and man page |
| grep | Search text inside files |

---

# What I Learned

- `find` is the most flexible search command.
- `locate` is faster but depends on an updated database.
- `which` finds executable paths.
- `whereis` provides additional locations.
- `grep` is useful for finding text patterns inside files.
