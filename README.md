# Email Threat Analysis – Phishing Simulation

## Overview
This project demonstrates a simulated email threat analysis workflow commonly performed by SOC and IT security analysts. A phishing email was generated in a controlled lab environment and analyzed using multiple industry-relevant tools.

Due to the use of a local SMTP testing environment, certain authentication results were simulated to reflect real-world phishing scenarios.

## Objectives
- Simulate a phishing email delivery
- Perform header analysis including SPF, DKIM, and DMARC review
- Analyze email body and social engineering techniques
- Perform attachment risk assessment
- Document findings in an incident-style report

## Tools Used
- MailHog (SMTP capture)
- Thunderbird (email client & header inspection)
- Sublime Text (raw header analysis)
- VirusTotal (hash-based attachment analysis)

## Key Findings
- Sender impersonation using a finance-themed email address
- Urgency-based social engineering language
- Missing or failed email authentication mechanisms (SPF, DKIM, DMARC)
- High-risk executable attachment delivered via email

## Outcome
The email was classified as a phishing attempt and would require quarantine and user awareness follow-up in a production environment.
