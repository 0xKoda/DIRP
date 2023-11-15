# DeFi Phishing Response Guide

### Table of Contents
- [Scope](#scope)
- [1. Preparation](#1-preparation)
- [2. Identification](#2-identification)
- [3. Response](#3-response)
- [4. Recovery](#4-recovery)

## Scope
<a id="scope"></a>
This playbook is specifically designed to address response to a phishing link being clicked.

```mermaid
Flowchart TD
    A[Start: Phishing Incident Response] --> B[Are DeFi Assets Drained?]
    B -- Yes --> C[Collect Transaction Hash]
    C --> D[Identify Address That Drained Assets]
    B -- No --> E[Continue Monitoring and Investigation]
    D --> F[Was the Transaction Signed Through a Webpage or Front End?]
    F -- Yes --> G[Note Domain Name]
    G --> H[Upload Domain to VirusTotal]
    H --> I[Make a Report to Alert Others]
    F -- No --> J[Further Investigate Transaction Source]
```

## 1. Preparation
<a id="1-preparation"></a>
<details>
<summary>Toggle for Details</summary>

- Compile a detailed inventory of 
    - all blockchain assets and domains controlled by the organization.
        - Crucial for avoiding errors with internal digital resources.
    - personnel authorized to manage blockchain domains and smart contracts.
- Formulate communication templates 
    - to quickly alert employees of ongoing phishing attacks targeting the company.
    - for collaboration with hosting and blockchain service providers against malicious entities.
    - to inform external stakeholders about potential security threats.

</details>

## 2. Identification
<a id="2-identification"></a>
<details>
<summary>Toggle for Details</summary>

- Educate staff on identifying DeFi phishing indicators, such as:
    - Unusual smart contract interactions.
    - Requests from unknown wallet addresses.
    - Unexpected transaction signing requests.
- Conduct frequent security reviews for:
    - Checking smart contract integrity.
    - Ensuring domain and wallet security.
    - Enhancing employee cyber awareness.

</details>

## 3. Response
<a id="3-response"></a>
<details>
<summary>Toggle for Details</summary>

- Immediate steps upon a phishing attack detection:
    - Secure and isolate affected assets and domains.
    - Alert internal security teams and start emergency protocols.
    - Issue organization-wide notifications to cease all blockchain-related operations temporarily.
- Liaise with blockchain networks or service providers for:
    - Assistance in tracking and halting malicious activities.
    - Support in recovering compromised assets, if possible.
    - Advice on fortifying security measures post-incident.

</details>

## 4. Recovery
<a id="4-recovery"></a>
<details>
<summary>Toggle for Details</summary>

- Analyze the incident to determine:
    - The point of entry and methods used in the phishing attack.
    - The full extent of damages, including asset loss and data compromise.
    - Necessary improvements in security protocols and staff training.
- Develop a recovery strategy encompassing:
    - Steps for safe resumption of all operations.
    - Preventative measures against future incidents.
    - Communication plans to restore trust with affected parties.

</details>
