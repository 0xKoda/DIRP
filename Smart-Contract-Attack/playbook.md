# Smart Contract Attack Response Guide

### Table of Contents
- [Scope](#scope)
- [1. Preparation](#1-preparation)
- [2. Identification](#2-identification)
- [3. Response](#3-response)
- [4. Recovery](#4-recovery)

## Scope
<a id="scope"></a>
This playbook is specifically designed to address response to a broad range of smart contract attacks.

```mermaid
flowchart TD
    A[Start: Identify] --> B[Are Contract Assets Drained?]
    B -- Yes --> C[Collect First Transaction Hash]
    C --> D[Identify Address That Drained Assets]
    B -- No --> E[Continue Monitoring and Investigation]
    D --> F[Is the contract pausible or upgradable?]
    F -- Yes --> G[Pause or upgrade the protocol]
    G --> H[Engage lawyer and communications plan]
    H --> I[Economic Analysis of patch to unpause]
    F -- No --> J[Investigate alternate measure to rescue funds]
```

## 1. Preparation
<a id="1-preparation"></a>
<details>
<summary>Toggle for Details</summary>

- **Audit and Review**: Regularly audit smart contracts for vulnerabilities.
- **Monitoring Measures**: Setup inhouse monitoring to help identification. 
- **Incident Response Team**: Establish an incident response team to engage in a war room scenario.
- **Pre-written Comms**: Engage legal team to draft pre-written comms to use in case of emergency.
- **Circuit Breakers**: Implement circuit breakers into smart contracts that can pause or prevent further loss. 
- **Maintain contact list**: Maintain a contact list with service providers and white-hats.

</details>

## 2. Identification
<a id="2-identification"></a>
<details>
<summary>Toggle for Details</summary>

- Identify the transaction hash that resulted from the smart contract attack:
    - Filter though unusual smart contract interactions.
    - Large transfer of assets.
- Identify the incident from monitoring capability:
    - Inhouse monitoring signals.
- Publicly Identified attack:
    - Members of the public have identified and alerted to the attack. 
    - A public security service has identified the attack.

</details>

## 3. Response
<a id="3-response"></a>
<details>
<summary>Toggle for Details</summary>

- Immediate steps following smart contract attack detection:
    - Secure and isolate affected assets and wallets.
    - Alert internal security teams and start emergency protocols.
    - Issue organization-wide notifications to cease all blockchain-related operations temporarily.
    - Pause any active contracts (if possible).
    - Begin sending any remaining assets to new hot-wallet or contract.
- Liaise with service providers from contact list for:
    - Assistance in tracking and halting malicious activities.
    - Support in recovering compromised assets, if possible.
    - Advice on fortifying security measures post-incident.
- Begin distributing pre-written communications:
    - Where possible have legal pre-read and authorize distribution.
    - Use social profiles to distribute initial statement.
- Begin engaging development team for patch if possible:
    - What are the economic impacts of a patch?
    - What are the knock on effects to other contracts?


</details>

## 4. Recovery
<a id="4-recovery"></a>
<details>
<summary>Toggle for Details</summary>

- Analyze the incident to determine:
    - The vulnerability that lead to the exploit.
    - The full extent of damages, including asset loss and data compromise (if any).
    - Necessary improvements in security protocols and staff training for prevention.
- Develop a recovery strategy encompassing:
    - Steps for safe resumption of all operations.
    - Stocktake of new and old contract addresses following incident.
    - Preventative measures against future incidents (bug bounties etc).
    - Communication plans to restore trust with affected parties.

</details>
