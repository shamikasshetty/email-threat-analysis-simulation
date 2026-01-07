# Incident Report – Email Threat Analysis

## Incident Summary
A suspected phishing email targeting an internal employee was identified and analyzed. The message impersonated an accounts payable department and attempted to deliver a potentially malicious attachment.

## Email Metadata
- From: ap@company-finance.com
- To: employee@company.com
- Subject: Invoice Pending Review – Immediate Action Required
- Delivery Method: Email (SMTP – simulated environment)

## Header Analysis
The email headers were reviewed using Thunderbird and Sublime Text. The analysis revealed the absence of valid SPF, DKIM, and DMARC authentication results. This prevents verification of the sender domain and increases the likelihood of spoofing.

> Note: Authentication headers were simulated to demonstrate real-world analysis, as the email was generated in a local SMTP environment.

## Body Analysis
The email content uses urgency, authority, and financial themes to pressure the recipient into opening the attachment without verification.

## Attachment Analysis
The attachment was delivered as an executable file, which represents a high-risk malware delivery method. Hash-based analysis was performed using VirusTotal to demonstrate threat intelligence correlation.

## Indicators of Compromise (IOCs)

| Type | Value |
|----|------|
| Sender Email | ap@company-finance.com |
| Subject | Invoice Pending Review |
| Attachment | Invoice_Review.exe |
| File Type | Executable |

## Verdict
Based on the observed indicators, this email is classified as a phishing attempt. Recommended actions include quarantining the message, blocking the sender domain, and conducting user awareness training.
