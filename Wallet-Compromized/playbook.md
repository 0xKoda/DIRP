# DeFi Wallet Compromize Incident Response Playbook

### Table of Contents
- [Scope](#scope)
- [1. Preparation](#1-preparation)
- [2. Identification](#2-identification)
- [3. Response](#3-response)
- [4. Recovery](#4-recovery)

## Scope
<a id="scope"></a>
This playbook is specifically designed to address response to a DeFi wallet compromize resulting in loss of funds.

```mermaid
flowchart TD
    A[Start: Wallet Compromise Response] --> B[Is There a Loss of Funds from the Wallet?]
    B -- Yes --> C[Identify Transaction Hash of Drained Funds]
    C --> D[Identify Addresses that Received Drained Assets]
    B -- No --> E[Continue Monitoring and Investigate Security Breach]
    D --> F[Was the Compromise a result of private key leak?]
    F -- Yes --> G[abstain from funding with large amounts of ETH for funds rescue]
    G --> H[Begin transfering remaining assets to new hotwallet]
    H --> I[Alert Stakeholders and Warn Users]
    F -- No --> J[Investigate Other Sources of Compromise]
```

## 1. Preparation
<a id="1-preparation"></a>
<details>
<summary>Toggle for Details</summary>

- Compile a detailed inventory of 
    - all blockchain assets and domains controlled by the organization.
        - Crucial for avoiding errors with internal digital resources.
    - personnel authorized to manage blockchain transactions and smart contracts.
- Formulate communication templates 
    - to inform external stakeholders about potential security threats.
- Create a new hot-wallet
    - write down seed phrase
    - quickly send any remaining funds from compromized wallet/s
- Implement wallet monitoring
    - monitor transactions and state changes accross wallets.
- Create an access list of employees who have access to seed phrases and private keys.

</details>

## 2. Identification
<a id="2-identification"></a>
<details>
<summary>Toggle for Details</summary>
- Monitoring alerts to loss of funds from wallet:
    
- Identify the transaction hash that resulted from the compormized wallet:
    - first transaction that drained funds.
    - receipt addresses.
    
- Identify the means which resulted in private key or seed phrase leak.
    - refer to [Stealer Malware](#) & [Phishing](../Phising/playbook.md)
    - private key hygiene
    - begin interviewing employees on access list

</details>

## 3. Response
<a id="3-response"></a>
<details>
<summary>Toggle for Details</summary>

- Immediate steps upon wallet drainage:
    - Avoid sending large amounts of ETH (or gas asset) to primary wallet.
    - Transfer any and all remaining funds and assets to the new hotwallet.
    - Alert internal security teams and start emergency protocols.
    - Issue organization-wide notifications to cease all blockchain-related operations temporarily.
    - Update any active contracts with new admin (if applicable).
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
    - The failures in security controls pertaining to wallet (key phrase, private keys).
    - The full extent of damages, funds audit.
    - Necessary improvements in security protocols and staff training for prevention.
- Develop a recovery strategy encompassing:
    - Steps for safe resumption of all operations.
    - Stocktake of new and old wallets following incident.
    - Preventative measures against future incidents.
    - Communication plans to restore trust with affected parties.

</details>
