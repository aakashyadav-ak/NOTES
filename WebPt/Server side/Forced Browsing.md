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

#### Types of Forced Browsing
```
┌─────────────────────────────────────────────────────────────────────────────┐
│                      FORCED BROWSING TYPES                                  │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│   1. Admin/Management Pages                                                 │
│      ├── /admin                                                             │
│      ├── /administrator                                                     │
│      ├── /manage                                                            │
│      ├── /dashboard                                                         │
│      └── /control-panel                                                     │
│                                                                             │
│   2. Backup & Configuration Files                                           │
│      ├── /backup/                                                           │
│      ├── /backup.zip                                                        │
│      ├── /config.php.bak                                                    │
│      ├── /database.sql                                                      │
│      └── /.env                                                              │
│                                                                             │
│   3. Debug & Development Endpoints                                          │
│      ├── /debug                                                             │
│      ├── /test                                                              │
│      ├── /phpinfo.php                                                       │
│      ├── /console                                                           │
│      └── /actuator (Spring Boot)                                            │
│                                                                             │
│   4. API Endpoints                                                          │
│      ├── /api/v1/admin/users                                                │
│      ├── /api/internal/config                                               │
│      ├── /api/debug/logs                                                    │
│      └── /swagger-ui.html                                                   │
│                                                                             │
│   5. Source Code & Version Control                                          │
│      ├── /.git/                                                             │
│      ├── /.svn/                                                             │
│      ├── /.hg/                                                              │
│      └── /src/                                                              │
│                                                                             │
│   6. Log Files                                                              │
│      ├── /logs/                                                             │
│      ├── /error.log                                                         │
│      ├── /access.log                                                        │
│      └── /debug.log                                                         │
│                                                                             │
│   7. Default Installation Files                                             │
│      ├── /readme.txt                                                        │
│      ├── /INSTALL.txt                                                       │
│      ├── /CHANGELOG.md                                                      │
│      └── /license.txt                                                       │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```