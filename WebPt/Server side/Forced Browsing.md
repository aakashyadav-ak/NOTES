Accessing pages/resources that exist but aren't linked in the UI by directly entering URLs

```
┌─────────────────────────────────────────────────────────────────┐
│                      FORCED BROWSING                            │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   Application has hidden/unlinked pages that attacker           │
│   discovers by guessing or brute-forcing URLs                   │
│                                                                 │
│                                                                 │
│   ┌──────────────────────────────────────────┐                  │
│   │            WEBSITE                       │                  │
│   │                                          │                  │
│   │   Visible Links:                         │                  │
│   │   ├── /home                              │                  │
│   │   ├── /about                             │                  │
│   │   ├── /contact                           │                  │
│   │   └── /login                             │                  │
│   │                                          │                  │
│   │   Hidden (But Accessible!):              │                  │
│   │   ├── /admin           ← Attacker finds! │                  │
│   │   ├── /backup          ← Attacker finds! │                  │
│   │   └── /config          ← Attacker finds! │                  │
│   │                                          │                  │
│   └──────────────────────────────────────────┘                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```