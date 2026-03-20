# VPN Troubleshooting Flowchart

flowchart TD
    A[User cannot connect to VPN] --> B{Internet works without VPN?}
    B -- No --> C[Resolve local connectivity first]
    B -- Yes --> D{Can user sign in to webmail or SSO?}
    D -- No --> E[Investigate account or password issue]
    D -- Yes --> F{MFA works?}
    F -- No --> G[Fix MFA issue]
    F -- Yes --> H{Exact VPN error known?}
    H -- No --> I[Collect screenshot or error text]
    H -- Yes --> J{Problem persists after restart and retry?}
    I --> J
    J -- No --> K[Resolved]
    J -- Yes --> L{Works on another network?}
    L -- Yes --> M[Likely local network issue]
    L -- No --> N{User authorized for VPN?}
    N -- No --> O[Submit or correct access request]
    N -- Yes --> P[Escalate to infrastructure or network team]