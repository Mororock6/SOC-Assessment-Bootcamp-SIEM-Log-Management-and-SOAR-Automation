# SOC Assessment Bootcamp – SIEM, Log Management and SOAR Automation

## Overview

This project was completed as part of a Security Operations Center (SOC) assessment bootcamp.

The objective was to build and validate a complete security monitoring workflow involving:

* Log Collection
* SIEM Integration
* Firewall Log Parsing
* Threat Intelligence Enrichment
* Security Orchestration and Automated Response (SOAR)

## Technologies Used

* Elastic Stack (Elasticsearch & Kibana)
* Winlogbeat
* Fluent Bit
* n8n
* VirusTotal API
* Windows Server
* FortiGate Logs

## Project Components

### 1. Windows Log Collection

Configured Winlogbeat to collect Windows Security Events including:

* Logon and Logoff Events
* Account Management Events
* Object Access Events
* Privilege Use Events
* System Events

Generated test events and successfully forwarded them to Elasticsearch.

### 2. Firewall Log Parsing

Developed a custom Fluent Bit parser capable of extracting key security fields from FortiGate firewall logs including:

* Source IP
* Destination IP
* Source Port
* Destination Port
* Service
* Action
* Malware Detection Information

Parsed logs were indexed and visualized within Kibana.

### 3. SOAR Automation

Designed and implemented an automated workflow using n8n that:

1. Retrieves logs from Elasticsearch
2. Extracts destination IP addresses
3. Removes duplicate values
4. Queries VirusTotal for reputation analysis
5. Generates automated email alerts for malicious IPs

## Skills Demonstrated

* SIEM Administration
* Log Management
* Security Monitoring
* Threat Intelligence
* Security Automation
* SOAR Development
* Elasticsearch
* Incident Detection
* Detection Engineering

## Outcome

Successfully integrated Windows logs, firewall logs, threat intelligence enrichment, and automated alerting into a single SOC workflow.

## Author

Amer Ashoush
CompTIA Security+ | ISC2 CC
