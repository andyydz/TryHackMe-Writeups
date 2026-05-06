# Linux Commands

## Overview
Linux commands are used to interact with the operating system through the terminal. They help users navigate directories, manage files, monitor processes, control permissions, and perform system administration tasks efficiently. Learning Linux commands is essential for cybersecurity, ethical hacking, and system administration.

---

# Navigation Commands

## pwd
Displays the current working directory.

```bash
pwd
```

---

## ls
Lists files and directories.

```bash
ls
ls -la
ls -lh
```
```
![ls Output](images/ls-output.png)

```

### Common Options
- `-l` → long listing format
- `-a` → show hidden files
- `-h` → human-readable file sizes

---

## cd
Changes the current directory.

```bash
cd Documents
cd ..
cd /
cd ~
```

### Examples
- `cd ..` → move one directory back
- `cd /` → go to root directory
- `cd ~` → go to home directory

---

# File Management Commands

## touch
Creates an empty file.

```bash
touch notes.txt
```

---

## mkdir
Creates a new directory.

```bash
mkdir test
mkdir projects
```

---

## rm
Removes files or directories.

```bash
rm file.txt
rm -r folder
rm -rf folder
```

### Important
- `-r` → recursive delete
- `-f` → force delete

---

## cp
Copies files and directories.

```bash
cp file.txt backup.txt
cp -r folder backup-folder
```

---

## mv
Moves or renames files.

```bash
mv old.txt new.txt
mv file.txt Documents/
```

---

## cat
Displays file contents.

```bash
cat file.txt
```

---

## nano
Opens the nano text editor.

```bash
nano notes.txt
```

### Nano Shortcuts
- `CTRL + O` → save
- `CTRL + X` → exit

---

## head
Displays first lines of a file.

```bash
head file.txt
```

---

## tail
Displays last lines of a file.

```bash
tail file.txt
tail -f logs.txt
```

---

# User Management Commands

## whoami
Displays current logged-in user.

```bash
whoami
```

---

## id
Displays user and group information.

```bash
id
```

---

## passwd
Changes user password.

```bash
passwd
```

---

## sudo
Executes commands with administrative privileges.

```bash
sudo apt update
```

---

# Permission Commands

## chmod
Changes file permissions.

```bash
chmod +x script.sh
chmod 755 file.sh
```

---

## chown
Changes ownership of files.

```bash
chown user:user file.txt
```

---

# System Information Commands

## uname
Displays system information.

```bash
uname -a
```

---

## hostname
Displays system hostname.

```bash
hostname
```

---

## top
Displays running processes and system usage.

```bash
top
```

---

## ps
Shows active processes.

```bash
ps aux
```

---

## df
Displays disk space usage.

```bash
df -h
```

---

## free
Displays memory usage.

```bash
free -h
```

---

# Networking Commands

## ping
Checks connectivity to another host.

```bash
ping google.com
```

---

## ip a
Displays IP addresses and interfaces.

```bash
ip a
```

---

## netstat
Displays network connections.

```bash
netstat -tulnp
```

---

## ssh
Connects securely to remote systems.

```bash
ssh user@192.168.1.10
```

---

# Package Management Commands

## apt update
Updates package lists.

```bash
sudo apt update
```

---

## apt upgrade
Upgrades installed packages.

```bash
sudo apt upgrade
```

---

## apt install
Installs packages.

```bash
sudo apt install nmap
```

---

# Searching Commands

## find
Searches for files and directories.

```bash
find /home -name file.txt
```

---

## grep
Searches text inside files.

```bash
grep "admin" users.txt
```

---

# Compression Commands

## zip
Compresses files.

```bash
zip files.zip file.txt
```

---

## unzip
Extracts zip files.

```bash
unzip files.zip
```

---

# What I Learned

- Linux terminal basics
- Navigating directories
- Managing files and folders
- Viewing and editing files
- Understanding permissions
- Managing users
- Monitoring processes
- Networking basics in Linux
- Installing packages
- Searching and compressing files

---

# Conclusion

Linux commands form the foundation of system administration and cybersecurity. Understanding these commands improves efficiency, troubleshooting skills, and practical knowledge required for ethical hacking and SOC operations.
