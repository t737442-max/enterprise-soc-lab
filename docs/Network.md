# Network Configuration

## Network Plan

| System | Role | IP |
|---|---|---|
| Splunk Server | SIEM | 192.168.1.10 |
| Windows Endpoint | Domain Client | 192.168.1.11 |
| Linux Router / Suricata IDS | Router / IDS | 192.168.1.30 |
| Linux Router (Internal) | Internal Network | 192.168.50.1 |
| Physical Network | LAN | 192.168.1.0/24 |

## Log Flow

Windows Server / Endpoint
→ Linux Router / Suricata IDS
→ Splunk Server

## Network Objective

Provide an isolated environment for controlled attack simulation, network monitoring, log collection, detection, and investigation.
