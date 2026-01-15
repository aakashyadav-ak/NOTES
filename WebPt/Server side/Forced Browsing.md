- Accessing pages/resources that exist but aren't linked in the UI by directly entering URLs

- Forced Browsing is accessing restricted or hidden pages by guessing the URL directly, rather than clicking a link provided by the website.

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