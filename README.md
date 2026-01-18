# Bounty-Hive Demo (Safe / Redacted)

This repo is a **public demo** of Bounty-Hive’s disclosure packaging model:
- **Safe-by-default** (no weaponized steps)
- **Redacted pre-purchase**
- **Lifecycle gated**: created → validated → approved → purchased → delivered
- **Audit-oriented**: packages reference artifacts by hash and signature placeholders

## What’s included

Two **sample disclosure packages** (fully redacted, non-actionable):

1) `demo/packages/sample-01-redacted-auth-bypass/`
   - Authorization boundary weakness (redacted)
   - Includes: `sealed_finding.json`, `redaction_manifest.json`, evidence + SARIF stubs

2) `demo/packages/sample-02-redacted-supply-chain/`
   - Dependency / build integrity concern (redacted)
   - Includes: `sealed_finding.json`, `redaction_manifest.json`, evidence + SARIF stubs

These are designed to show **structure, governance, and custody** without revealing exploitation details.

## Why this matters

Most vulnerability workflows fail at trust:
- Findings get emailed around without tamper-evidence
- Repro steps leak too early
- There’s no enforceable lifecycle or entitlement boundary

Bounty-Hive treats every sensitive artifact as:
- **created** (sealed + redacted)
- **validated** (defensive confirmation only)
- **approved** (governance decision + policy snapshot)
- **purchased** (entitlement granted)
- **delivered** (full package released to the customer only)

## What you can safely evaluate here

- Package structure and intended schema boundaries
- Redaction behavior (what exists pre-purchase vs post-purchase)
- How artifacts are referenced (hash-first mindset)
- How lifecycle states constrain what can be shared

## What you will NOT find here

- No exploitation steps
- No payloads
- No endpoint/parameter specifics
- No real targets or identifying logs
- No “how to break in” content

## Next steps (for pilot conversations)

If you’re evaluating a pilot:
- We can run a **scope-controlled** engagement
- You receive **redacted findings immediately**
- Full delivery is gated by **approval + purchase**
- Everything is **auditable and entitlement-bound**

---

**Non-Blocking Disclaimer**
This demo is for authorized defensive vulnerability disclosure workflows only.
