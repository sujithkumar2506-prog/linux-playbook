
# Linux Basic Commands

A quick reference to essential Linux commands for system information, user identification, and basic network operations.

## 1. User Information

| Command | Purpose |
|---|---|
| `whoami` | Displays the username of the currently logged-in user. |
| `who` | Displays users currently logged into the system. |
| `id` | Displays the current user's UID, GID, and group memberships. |
| `logname` | Displays the original login username. |

## 2. Host & OS Information

| Command | Purpose |
|---|---|
| `hostname` | Displays the hostname of the machine. |
| `hostnamectl` | Displays hostname, OS, kernel, and architecture information. |
| `uname -a` | Displays complete kernel and system information. |
| `uname -r` | Displays the Linux kernel version. |
| `uname -m` | Displays the machine hardware architecture. |
| `uname -s` | Displays the kernel name. |
| `cat /etc/os-release` | Displays the Linux distribution and OS version. |

## 3. File & Directory Information

| Command | Purpose |
|---|---|
| `pwd` | Displays the current working directory. |
| `ls` | Lists files and directories in the current directory. |
| `ls -la` | Lists all files, including hidden files, with detailed information. |

## 4. Network & Connectivity

| Command | Purpose |
|---|---|
| `ping <host>` | Checks network reachability of a remote host using ICMP. |
| `curl <URL>` | Transfers data to or from a server using a specified URL. |
| `curl -I <URL>` | Retrieves HTTP response headers without downloading the response body. |
| `wget <URL>` | Downloads files from a remote server. |

## 5. Useful Command References

| Command | Purpose |
|---|---|
| `man <command>` | Opens the manual page for a command. |
| `<command> --help` | Displays usage instructions and available options for a command. |
| `clear` | Clears the terminal screen. |

---

## Important Notes

- `whoami` identifies the current effective user.
- `who` shows logged-in sessions.
- `hostname` identifies the machine.
- `/etc/os-release` identifies the Linux distribution.
- `uname` provides kernel-related information.
- `ping`, `curl`, and `wget` serve different networking purposes.
