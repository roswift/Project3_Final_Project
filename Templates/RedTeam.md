# Red Team: Summary of Operations

## Table of Contents
- Exposed Services
- Critical Vulnerabilities
- Exploitation

### Exposed Services

Nmap scan results for each machine reveal the below services and OS details:

```bash
nmap -sS -A 192.168.1.110
```
![nmap1](../images/nmap1.JPG)
![nmap2](../images/nmap2.JPG)


This scan identifies the services below as potential points of entry:

`Target 1`

| **PORT** | **Port Status** | **Service** |                    **Version**                   |
|:--------:|:---------------:|:-----------:|:------------------------------------------------:|
| 22/tcp   | open            | ssh         | OpenSSH 6.7 Debian 5+deb8u4 (protocol 2.0)       |
| 80/tcp   | open            | http        | Apache httpd 2.4.10 ((Debian))                   |
| 111/tcp  | open            | rpcbind     | 2-4 (RPC #100000)                                |
| 139/tcp  | open            | netbios-ssn | Samba 3.X - 4.X (workgroup: WORKGROUP)           |
| 445/tcp  | open            | netbios-ssn | Sambra smbd 4.2.14-Debian (workgroup: WORKGROUP) |

The following vulnerabilities were identified on each target:
- `Target 1`
  - List of
  - Critical
  - Vulnerabilities

_TODO: Include vulnerability scan results to prove the identified vulnerabilities._

### Exploitation
_TODO: Fill out the details below. Include screenshots where possible._

The Red Team was able to penetrate `Target 1` and retrieve the following confidential data:
- Target 1
  - `flag1.txt`: _TODO: Insert `flag1.txt` hash value_
    - **Exploit Used**
      - _TODO: Identify the exploit used_
      - _TODO: Include the command run_
  - `flag2.txt`: _TODO: Insert `flag2.txt` hash value_
    - **Exploit Used**
      - _TODO: Identify the exploit used_
      - _TODO: Include the command run_
