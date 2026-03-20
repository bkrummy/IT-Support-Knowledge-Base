# Printer Troubleshooting Flowchart

flowchart TD
    A[User cannot print] --> B{One user or many users?}
    B -- Many --> C[Check printer or print server outage]
    B -- One --> D{Correct printer selected?}
    D -- No --> E[Select correct printer and retest]
    D -- Yes --> F{Printer online and powered on?}
    F -- No --> G[Restore power or network connection]
    F -- Yes --> H{Jobs stuck in queue?}
    H -- Yes --> I[Clear queue and restart spooler]
    H -- No --> J{Driver or mapping issue suspected?}
    J -- Yes --> K[Re-add printer or reinstall driver]
    J -- No --> L[Test print from simple app]
    L --> M{Still failing?}
    M -- No --> N[Resolved]
    M -- Yes --> O[Escalate to printer hardware or print server support]