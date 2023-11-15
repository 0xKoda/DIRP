
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