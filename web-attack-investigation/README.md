# Web Attack Detection & Investigation

## Project Overview

This project demonstrates a Security Operations Center (SOC) investigation of suspicious web activity using Splunk SIEM.

The lab simulates automated web path enumeration targeting a web application through repeated HTTP GET requests to PHP and administrative endpoints.

**Note:** This is an independent educational project using fictional data. No company logs, infrastructure details, or customer information are included.

## Scenario

A web application receives a high volume of HTTP requests from an external source.

The activity includes:
- Repeated requests to different PHP files.
- Attempts to access administrative paths.
- Requests to WordPress-related directories.
- Multiple HTTP 404 responses.

## Investigation Objectives

- Identify suspicious web traffic.
- Analyze HTTP response codes.
- Identify unusual request patterns.
- Investigate potential reconnaissance activity.
- Map findings to MITRE ATT&CK.
- Recommend defensive actions.

## Tools & Technologies

- Splunk Enterprise / Splunk Enterprise Security
- Search Processing Language (SPL)
- Nginx Logs
- MITRE ATT&CK

## Key Skills Demonstrated

- SIEM Alert Investigation
- Log Analysis
- Threat Detection
- Web Attack Analysis
- Incident Documentation
- Security Recommendations

## Project Structure

Project files will include:
- Incident Investigation Report
- SPL Queries
- Investigation Findings
- MITRE ATT&CK Mapping

## Disclaimer

This project is intended for educational and portfolio purposes only. All indicators, IP addresses, domains, and event data used in the public lab documentation are fictional or sanitized.
