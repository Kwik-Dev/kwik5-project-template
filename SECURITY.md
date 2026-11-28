# Security

## Reporting a vulnerability

Use GitHub's **Private vulnerability reporting** on this repository (Security → Report a
vulnerability), or email **support@kwiksher.com**. An advisory is preferred: it stays private from
the first message and we can fix, release and disclose in one place.

Please do not open a public issue for a vulnerability. We aim to answer within a week.

## What this repository holds, and what it cannot leak

* **The template is data and assets.** It runs inside a user's book, but it holds no credentials, no
  endpoint of ours, and no licence check.
* **`version.txt` is a contract.** `requires.cli` is enforced by the CLI before an install, so a
  template that claims a floor it does not need is a bug worth reporting, not a nicety.
* **Assets carry provenance.** `Solar2D/README.md` lists the vendored libraries and their licences;
  a new asset without a licence line is not merged.

## Supported versions

The latest release of each channel is supported. Kwik is pre-1.0 where it is pre-1.0 — the
`version.txt` a release stamps and `kwik version` are the truth; older tags are not patched.

## Not a security boundary

Kwik's paid product is **Kwik Cloud** (GPU time and the credit ledger). Everything in this
repository runs on the user's machine and talks to no server of ours except where the user configures
one — so a bug here is a local bug, not a leak of someone else's data.
