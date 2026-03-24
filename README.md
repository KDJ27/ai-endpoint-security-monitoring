# AI-Powered Endpoint Security Monitoring & Response (Homelab)

## Overview

This project demonstrates a lightweight, automated endpoint security monitoring and response system built using n8n and Windows telemetry.

The system continuously monitors a Windows 11 asset, detects suspicious activity, and triggers real-time alerts using automation workflows.

## Architecture

Windows 11 Endpoint → PowerShell Telemetry → n8n Automation Engine → Detection Logic → Discord Alerts

## Features

* Real-time endpoint monitoring
* Automated detection of suspicious activity
* Event-driven alerting system
* Scalable automation workflows

## Detection Use Cases

* Failed login attempts (brute-force detection)
* Windows Defender disabled detection
* Disk usage anomaly detection
* Endpoint heartbeat monitoring

## Technologies Used

* n8n (workflow automation)
* PowerShell (endpoint telemetry)
* Windows Event Logs
* Docker (self-hosted environment)
* Discord Webhooks (alerting)

## How It Works

1. PowerShell script collects system and security data from a Windows 11 machine.
2. Data is sent to n8n via a webhook.
3. n8n processes the data and evaluates detection rules.
4. Alerts are triggered based on defined conditions.

## Simulated Attacks

To validate detection capabilities, the following scenarios were simulated:

* Brute-force login attempts
* Windows Defender disablement
* Disk usage anomalies

## Example Alert

🚨 Windows 11 alert detected

* Failed logins: 10
* Defender status: Disabled
* Disk usage: 92%

## Future Improvements

* AI-based event classification
* Multi-endpoint monitoring
* Automated containment actions
* Integration with SIEM platforms

## Screenshots

(see /screenshots folder)

## Disclaimer

This project was built in a controlled homelab environment for educational and demonstration purposes only.
