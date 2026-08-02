# Linux Process Management and System Monitoring

## Overview

A process is a running instance of a program. Linux provides commands to monitor, manage, and terminate processes.

---

## ps

Displays information about running processes.

```bash
ps
```

Show all running processes:

```bash
ps -e
```

Detailed process list:

```bash
ps -ef
```

---

## top

Displays real-time information about CPU, memory, and running processes.

```bash
top
```

Useful keys while `top` is running:

- `q` → Quit
- `k` → Kill a process
- `P` → Sort by CPU usage
- `M` → Sort by Memory usage

---

## htop

An interactive version of `top`.

```bash
htop
```

Install (Ubuntu/Debian):

```bash
sudo apt install htop
```

---

## kill

Terminates a process using its Process ID (PID).

```bash
kill 1234
```

Force terminate:

```bash
kill -9 1234
```

---

## pgrep

Finds the PID of a process.

```bash
pgrep firefox
```

---

## pkill

Terminates processes by name.

```bash
pkill firefox
```

---

## free

Displays memory usage.

```bash
free -h
```

Example output:

```text
              total        used        free
Mem:          7.6Gi       2.1Gi       4.3Gi
```

---

## df

Displays disk space usage.

```bash
df -h
```

---

## du

Displays directory size.

```bash
du -sh Documents
```

---

## uptime

Shows how long the system has been running.

```bash
uptime
```

---

## Common Commands

| Command | Purpose |
|---------|---------|
| ps | View running processes |
| top | Real-time process monitoring |
| htop | Interactive process viewer |
| kill | Terminate a process |
| pgrep | Find process ID |
| pkill | Kill process by name |
| free | Memory usage |
| df | Disk usage |
| du | Directory size |
| uptime | System uptime |

---

# Practice Examples

View all running processes:

```bash
ps -ef
```

Monitor system performance:

```bash
top
```

Check memory usage:

```bash
free -h
```

Check disk usage:

```bash
df -h
```

Display the size of the Downloads folder:

```bash
du -sh Downloads
```

---

# What I Learned

- Every running program is a process.
- `ps` and `top` help monitor processes.
- `kill` and `pkill` terminate processes.
- `free` displays memory usage.
- `df` and `du` help monitor disk usage.
- Process management is an essential skill for Linux and cloud administrators.
