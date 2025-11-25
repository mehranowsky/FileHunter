# FileHunter

FileHunter is a lightweight and simplified alternative to the BackupKiller tool.  
It generates backup-file wordlists related to a given domain (e.g., `example.com.zip`, `example.zip~`, etc.).  
Designed for bug hunters who want a fast way to enumerate domain-based backup filenames.

---

## Features

- Generates backup filename variations based on a target domain  
- Lightweight and fast  
- Simple command-line interface  
- Optional Date Mode for date-based backup combinations  

---

## Usage

```bash
# Usage
filehunter -h
usage: fileHunter.py [-h] -d D [-dm] -w W

options:
  -h, --help  show this help message and exit
  -d D        The target domain name
  -dm         Date mode
  -w W        Wordlist.json, wordpress.json 
```

# Examples
```
# Generate backup filenames from a domain with simple wordlist
filehunter -d example.com -w wordlist.json

# Generate with Date Mode enabled and wordpress wordlist
filehunter -d example.com -dm -w wordpress.json
```

# Sample Output
```
example.com.zip
example.zip~
example_com_backup.tar.gz
example-2024-11-25.bak
