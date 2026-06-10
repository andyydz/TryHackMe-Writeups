# Windows PowerShell

This folder contains my notes and write-ups related to Windows PowerShell and PowerShell scripting.

The purpose of these write-ups is to develop a strong understanding of PowerShell automation, scripting, system administration, process analysis, and security operations.

PowerShell is one of the most powerful tools available for Windows administration and cybersecurity operations.

---

# Topics Covered

## 1. Introduction to PowerShell

Understanding Microsoft's command-line and automation framework.

### Key Concepts

- PowerShell basics
- Cmdlets
- Object-oriented output
- Automation

### Example

```powershell
Get-Help
Get-Command
```

### Use Cases

- Administration
- Automation
- Security operations

---

## 2. Navigating the File System

Working with files and directories using PowerShell.

### Key Concepts

- File navigation
- Directory management
- File manipulation

### Example

```powershell
Get-ChildItem
Set-Location
```

### Use Cases

- File investigations
- Log analysis
- Administrative tasks

---

## 3. Working with Files

Managing files through PowerShell commands.

### Key Concepts

- Creating files
- Copying files
- Moving files
- Removing files

### Example

```powershell
New-Item
Copy-Item
Move-Item
Remove-Item
```

### Use Cases

- Automation
- File management
- System maintenance

---

## 4. Piping, Filtering, and Sorting Data

Understanding PowerShell's object pipeline.

### Key Concepts

- Pipelines
- Filtering
- Sorting
- Data processing

### Example

```powershell
Get-Process | Sort-Object CPU
```

### Use Cases

- Data analysis
- Threat hunting
- System monitoring

---

## 5. System and Network Information

Gathering detailed information about Windows systems.

### Key Concepts

- System information
- Network configuration
- Services
- Hardware details

### Example

```powershell
Get-ComputerInfo
Get-NetIPAddress
```

### Use Cases

- Auditing
- Asset management
- Incident response

---

## 6. Real-Time System Analysis

Monitoring active processes and services.

### Key Concepts

- Process analysis
- Service monitoring
- Event logs

### Example

```powershell
Get-Process
Get-Service
```

### Use Cases

- Threat hunting
- Malware investigations
- Performance monitoring

---

## 7. PowerShell Scripting

Automating tasks using PowerShell scripts.

### Key Concepts

- Variables
- Loops
- Conditions
- Script execution

### Example

```powershell
$Name = "Andrew"
Write-Output "Hello $Name"
```

### Use Cases

- Automation
- Reporting
- Security monitoring

---

# Skills Learned

- PowerShell fundamentals
- PowerShell scripting
- Automation techniques
- Process analysis
- Data filtering
- Windows administration

---

# Why PowerShell Matters in Cybersecurity

PowerShell is heavily used in:

- SOC Operations
- Threat Hunting
- Incident Response
- Blue Team Operations
- Security Automation
- Digital Forensics

---

# Platform

- TryHackMe
- Windows Virtual Machines
- GitHub

---

# Author

Andrew D Souza

Cybersecurity Learner | PowerShell | Blue Team | TryHackMe
