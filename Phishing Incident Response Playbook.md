graph TD
    A[Start: Phishing Alert Received] --> B{Did User Click Link?}
    B -- Yes --> C[Isolate Workstation]
    B -- No --> D{Is there an Attachment?}
    
    C --> E[Reset User Credentials]
    E --> F[Check for Lateral Movement]
    
    D -- Yes --> G[Submit to Sandbox/VirusTotal]
    D -- No --> H[Analyze Email Headers/IPs]
    
    G --> I{Is it Malicious?}
    I -- Yes --> C
    I -- No --> J[Close Alert as Benign]
    
    H --> K[Block Sender IP/Domain]
    K --> L[Purge Email from Inbox]
    L --> M[Post-Incident Review]
