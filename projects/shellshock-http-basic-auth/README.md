# Shellshock and HTTP Basic Auth

## Overview
This project documents two network-focused investigation labs based on PCAP analysis: a Shellshock-related web attack and an HTTP Basic Authentication case.  
The objective was to inspect HTTP traffic, identify suspicious behavior, extract technical evidence, and understand how insecure or malicious web activity appeared at packet level.

## Scenario
Both exercises were based on packet capture analysis in a SOC-style context.  
The investigation focused on HTTP requests, server responses, headers, authentication behavior, and attacker-controlled input visible in network traffic.

## Objectives
- Analyze suspicious HTTP activity in PCAP files.
- Identify evidence of exploit attempts against a web server.
- Review server and application details exposed in HTTP headers.
- Understand how HTTP Basic Authentication exposes credentials when used without encryption.

## Tools Used
- Wireshark
- PCAP analysis
- HTTP traffic inspection
- Header analysis
- Basic authentication review
- Base64 decoding concepts

## Investigation Areas

### 1. Shellshock Attack Analysis
The PCAP was reviewed to identify suspicious HTTP requests associated with a Shellshock-style exploit attempt.  
The investigation focused on attacker-supplied input, abnormal request structure, and server-side behavior visible in HTTP traffic.

### 2. HTTP Basic Authentication Analysis
The traffic was inspected to identify how credentials were transmitted during HTTP Basic Authentication.  
This analysis highlighted that credentials can be recovered from network traffic when Basic Authentication is used without transport-layer protection.

## Key Findings
- Suspicious HTTP requests can reveal exploit attempts against web applications and servers.
- HTTP headers can expose useful server details such as platform, software, and version information.
- Packet captures can provide enough evidence to reconstruct attacker behavior and request flow.
- HTTP Basic Authentication is insecure over unencrypted traffic because credentials are only encoded, not securely protected.

## Outcome
This project strengthened my ability to analyze packet captures, investigate web-based attacks, and interpret HTTP-level evidence during an incident.  
It also reinforced the importance of recognizing weak authentication mechanisms and attacker activity directly from network traffic.

## Skills Demonstrated
- PCAP analysis
- HTTP traffic analysis
- Web attack investigation
- Shellshock-related request analysis
- Basic authentication analysis
- Technical documentation
