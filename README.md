```
╔══════════════════════════════════════════════════════════════════════════════╗
║                                                                              ║
║   ██╗    ██╗ █████╗ ██████╗ ██╗      ██████╗  ██████╗██╗  ██╗                ║
║   ██║    ██║██╔══██╗██╔══██╗██║     ██╔═══██╗██╔════╝██║ ██╔╝                ║
║   ██║ █╗ ██║███████║██████╔╝██║     ██║   ██║██║     █████╔╝                 ║
║   ██║███╗██║██╔══██║██╔══██╗██║     ██║   ██║██║     ██╔═██╗                 ║
║   ╚███╔███╔╝██║  ██║██║  ██║███████╗╚██████╔╝╚██████╗██║  ██╗                ║
║    ╚══╝╚══╝ ╚═╝  ╚═╝ ╚═╝  ╚═╝╚══════╝ ╚═════╝  ╚═════╝╚═╝  ╚═╝                ║
║                                                                              ║
║              P A S S W O R D   S T A N D A R D   v 0 . 1 . 0                 ║
║                                                                              ║
║   ─────────────────────────────────────────────────────────────────────────  ║
║   Status: COMPLIANT          Entropy: ∞          Field Limit: cope harder    ║
║   ─────────────────────────────────────────────────────────────────────────  ║
║                                                                              ║
╚══════════════════════════════════════════════════════════════════════════════╝
```

```
┌──[ THE STANDARD ]────────────────────────────────────────────────────────────┐
│                                                                              │
│   Every compliant password MUST satisfy all five requirements:               │
│                                                                              │
│   [ 1 ]  ≥ 247 characters                                                    │
│   [ 2 ]  Contains a differential equation                                    │
│   [ 3 ]  Contains a prime number you can defend philosophically              │
│   [ 4 ]  Follows an anti-hero story arc                                      │
│   [ 5 ]  Ends with an M. Night Shyamalan plot twist                          │
│                                                                              │
│   Failure to comply will be reported to the Compliance Gremlin (the auditor  │
│   who lives behind the breakroom microwave).                                 │
│                                                                              │
└──────────────────────────────────────────────────────────────────────────────┘
```

```
┌──[ INSTALL ]─────────────────────────────────────────────────────────────────┐
│                                                                              │
│   > Personal install (all projects):                                         │
│                                                                              │
│     git clone https://github.com/grcwarlock/warlock-password.git             │
│     mkdir -p ~/.claude/skills                                                │
│     cp -r warlock-password ~/.claude/skills/warlock-password                 │
│                                                                              │
│   > Or symlink so the skill updates when you `git pull`:                     │
│                                                                              │
│     ln -s "$(pwd)/warlock-password" ~/.claude/skills/warlock-password        │
│                                                                              │
│   > Project-level install (this repo only):                                  │
│                                                                              │
│     mkdir -p .claude/skills                                                  │
│     cp -r warlock-password .claude/skills/warlock-password                   │
│                                                                              │
│   Restart your Claude Code session. The skill auto-registers.                │
│                                                                              │
└──────────────────────────────────────────────────────────────────────────────┘
```

```
┌──[ USAGE ]───────────────────────────────────────────────────────────────────┐
│                                                                              │
│   Trigger phrases:                                                           │
│                                                                              │
│     "generate a warlock password"                                            │
│     "give me a 247-character password"                                       │
│     "make me a password with a story arc"                                    │
│     "i need a password with a Shyamalan twist"                               │
│     "generate a philosophically defensible prime password"                   │
│                                                                              │
│   Example session:                                                           │
│                                                                              │
│     user@terminal:~$ generate a warlock password                             │
│                                                                              │
│     <password>                                                               │
│     [247+ characters of single-string narrative containing a verified        │
│      prime, derivative notation, an anti-hero arc, and a recursive twist]    │
│     </password>                                                              │
│                                                                              │
│     LENGTH: 263                                                              │
│                                                                              │
│     NARRATIVE SUMMARY (memory aid only — do NOT use as the password):        │
│      - Prime:    4327                                                        │
│      - Equation: d²y/dx² + 3(dy/dx) − 7y = 0                                 │
│      - Arc:      auditor forges audit trail to protect colleague,            │
│                  realizes colleague was the one being audited                │
│      - Twist:    the auditor was their own past self, sent back              │
│                  through the records they had been forging                   │
│                                                                              │
└──────────────────────────────────────────────────────────────────────────────┘
```

```
┌──[ KNOWN ISSUES ]────────────────────────────────────────────────────────────┐
│                                                                              │
│   • Most password fields cap at 64 or 128 characters.                        │
│     This is part of the joke. The fields are wrong, not the password.        │
│                                                                              │
│   • Your password manager may experience an existential crisis.              │
│     This is normal. Offer it tea.                                            │
│                                                                              │
│   • The Shyamalan twist may cause your IT manager to re-evaluate             │
│     several life choices. There is no patch.                                 │
│                                                                              │
│   • Differential equations rendered in standard mathematical notation        │
│     may be flagged by SQL injection filters that have never seen joy.        │
│                                                                              │
└──────────────────────────────────────────────────────────────────────────────┘
```

```
┌──[ DO NOT ]──────────────────────────────────────────────────────────────────┐
│                                                                              │
│   ✗ Use these passwords for anything that actually matters.                  │
│   ✗ Paste one into your bank's login form and email me the screenshot.       │
│   ✗ Recite a generated password aloud near a Mersenne prime enthusiast.      │
│   ✗ Try to "improve" the twist. The model has tried. The model has failed.  │
│                                                                              │
└──────────────────────────────────────────────────────────────────────────────┘
```

```
┌──[ CONTRIBUTING ]────────────────────────────────────────────────────────────┐
│                                                                              │
│   PRs welcome, especially:                                                   │
│                                                                              │
│     [+] New forbidden twist clichés the model keeps reaching for             │
│     [+] Reports of pseudoprimes sneaking past verification                   │
│     [+] Reports of plain algebraic equations posing as differential ones     │
│     [+] Genre packs (noir, cosmic horror, corporate thriller, regency)       │
│                                                                              │
│   Open issues with the label [compliance-gremlin] for behavioral bugs.       │
│                                                                              │
└──────────────────────────────────────────────────────────────────────────────┘
```

```
╔══════════════════════════════════════════════════════════════════════════════╗
║  LICENSE: MIT     │   STATUS: SHIPPED     │   THREAT MODEL: yes              ║
║  F1 HELP   F2 INSTALL   F3 USAGE   F5 RECOMPILE   F10 ACCEPT YOUR FATE       ║
╚══════════════════════════════════════════════════════════════════════════════╝
```
