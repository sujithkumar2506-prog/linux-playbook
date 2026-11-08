
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

### RPM (Red Hat Package Manager)

RPM is a low-level package management tool used in Red Hat-based Linux distributions.

It works with `.rpm` package files and can install, query, upgrade, and remove packages.

**Important RPM Commands**

| Command | Purpose |
|---|---|
| `rpm -ivh package.rpm` | Install an RPM package |
| `rpm -e package_name` | Remove an installed package |
| `rpm -qa` | List all installed RPM packages |
| `rpm -q package_name` | Check whether a package is installed |

### DNF (Dandified YUM)

DNF is a high-level package manager used in Red Hat-based Linux distributions.

It downloads packages from repositories and automatically handles dependencies.

**Important DNF Commands**

| Command | Purpose |
|---|---|
| `sudo dnf install package_name` | Install a package |
| `sudo dnf remove package_name` | Remove a package |
| `dnf list installed` | List all installed packages |
| `dnf list installed package_name` | Check whether a specific package is installed |
| `sudo dnf upgrade` | Update installed packages |

### RPM vs DNF

| RPM | DNF |
|---|---|
| Low-level package management tool | High-level package manager |
| Works with local `.rpm` files | Downloads packages from repositories |
| Does not automatically resolve dependencies | Automatically resolves dependencies |
| Useful for direct package operations | Useful for everyday software management |

**Real-world analogy:**

- RPM is like manually installing software using an installation file.
- DNF is like an app store that downloads software and handles its requirements automatically.

**Remember:** DNF uses RPM underneath to manage `.rpm` packages.