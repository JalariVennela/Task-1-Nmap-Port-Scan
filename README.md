# Task-1-Nmap-Port-Scan
Cyber Security Internship Task 1 - Network Port Scanning using Nmap
# Task 1: Scan Your Local Network for Open Ports

## Objective
The objective of this task is to scan the local network using Nmap, identify active devices, detect open TCP ports, and understand the security risks associated with exposed network services.

## Tool Used
- Nmap 7.99
- Windows Command Prompt

## Network Information
- Network Range: 10.95.138.0/24
- Scan Type: TCP SYN Scan (-sS)

## Command Used

```bash
nmap -sS 10.95.138.0/24
```

## Scan Results

### Active Hosts
- 3 hosts were detected.

### Open Ports

#### Host: 10.95.138.199
| Port | Service |
|------|---------|
|53|DNS|
|7000|AFS File Server|

#### Host: 10.95.138.206
| Port | Service |
|------|---------|
|135|MSRPC|
|139|NetBIOS Session Service|
|445|Microsoft-DS (SMB)|

## Security Analysis

- Port 53 is used for DNS services.
- Port 7000 is associated with AFS file services.
- Port 135 is used by Windows RPC.
- Port 139 supports NetBIOS file sharing.
- Port 445 supports SMB file sharing and should be protected because it has been targeted by malware in the past.

## Conclusion

The network scan successfully identified active devices and open TCP ports. This task helped in understanding network reconnaissance, port scanning, and basic network security concepts.
