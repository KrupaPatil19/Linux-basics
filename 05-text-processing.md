# Linux Text Processing Commands

## Overview

Linux provides powerful command-line tools to process, filter, and manipulate text efficiently.

---

## cat

Displays the contents of a file.

```bash
cat file.txt
```

Display line numbers:

```bash
cat -n file.txt
```

---

## head

Displays the first 10 lines of a file.

```bash
head file.txt
```

Display the first 5 lines:

```bash
head -5 file.txt
```

---

## tail

Displays the last 10 lines of a file.

```bash
tail file.txt
```

Display the last 5 lines:

```bash
tail -5 file.txt
```

Monitor a log file in real time:

```bash
tail -f application.log
```

---

## wc

Counts lines, words, and characters.

```bash
wc file.txt
```

Count only lines:

```bash
wc -l file.txt
```

Count only words:

```bash
wc -w file.txt
```

---

## sort

Sorts lines alphabetically.

```bash
sort names.txt
```

Reverse order:

```bash
sort -r names.txt
```

---

## uniq

Removes duplicate consecutive lines.

```bash
uniq data.txt
```

Count duplicate occurrences:

```bash
uniq -c data.txt
```

---

## cut

Extracts specific columns from a file.

```bash
cut -d ":" -f1 /etc/passwd
```

---

## tr

Translates or replaces characters.

Convert lowercase to uppercase:

```bash
echo "linux" | tr 'a-z' 'A-Z'
```

Output:

```text
LINUX
```

---

## paste

Merges lines from multiple files.

```bash
paste names.txt ages.txt
```

---

## Common Commands

| Command | Purpose |
|---------|---------|
| cat | Display file contents |
| head | Show beginning of file |
| tail | Show end of file |
| wc | Count lines, words, characters |
| sort | Sort text |
| uniq | Remove duplicates |
| cut | Extract fields |
| tr | Translate characters |
| paste | Merge files |

---

# Practice Examples

Display the first 20 lines:

```bash
head -20 notes.txt
```

Count words:

```bash
wc -w report.txt
```

Sort a file:

```bash
sort students.txt
```

Convert text to uppercase:

```bash
echo "hello world" | tr 'a-z' 'A-Z'
```

---

# What I Learned

- Linux provides powerful tools for working with text.
- Commands can be combined using pipes (`|`) to build efficient workflows.
- Text processing commands are commonly used in scripting and log analysis.
