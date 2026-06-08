# Security Policy

Security is the core of what we build at Noru. We take vulnerabilities in our products,
services, and open-source code seriously and appreciate responsible disclosure.

This policy mirrors our [Security Page](https://noru.tech/security). The full
[disclosure policy and rules of engagement](https://noru.tech/security/disclosure-policy)
and our machine-readable [`security.txt`](https://noru.tech/.well-known/security.txt) are
published on our website.

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues, discussions,
or pull requests.**

Instead, report them privately through one of the following channels:

1. **Security contact (preferred)** — Email our security team at `security@noru.tech`. For
   sensitive reports, encrypt your submission with our
   [PGP key](https://noru.tech/.well-known/pgp-key.asc).
2. **GitHub Private Vulnerability Reporting** — Use the **"Report a vulnerability"** button
   under the **Security** tab of the affected repository. This opens a private advisory
   visible only to maintainers.

To help us validate and remediate quickly, please include:

- Clear reproduction steps and the impacted endpoints or workflows.
- The affected repository, version, commit, or endpoint.
- Evidence that distinguishes a genuine security boundary from expected behavior.
- Proof-of-concept or exploit code, and screenshots, if available.
- The impact, including how an attacker might exploit it.
- Contact details so we can follow up during remediation.

Please avoid sending sensitive personal data unless it is absolutely necessary to
demonstrate the issue.

## Our Commitment

When you report a vulnerability responsibly, we will:

- **Acknowledge** receipt within **24 hours**.
- Provide **initial triage** within **3 business days**.
- Keep you informed of remediation progress.
- Work toward **coordinated disclosure** within **90 days**, adjusted as needed to protect
  customer safety.
- Credit you in the advisory and our
  [Hall of Fame](https://noru.tech/security/hall-of-fame) once the issue is resolved,
  unless you prefer to remain anonymous.

## Scope

This policy applies to all repositories under the `noru-tech` organization. For
vulnerabilities in the hosted Noru platform itself, the same private channels apply.
Details on our security program and controls are available in our
[Trust Center](https://trust.noru.tech).

## Safe Harbor

We authorize good-faith security research and will not pursue legal action against
researchers who:

- Act in good faith and follow this policy.
- Avoid privacy violations and service degradation, and do not exfiltrate data.
- Do not access or modify data that does not belong to them.
- Stop testing and report immediately once a vulnerability is confirmed.
- Give us reasonable time to remediate before any public disclosure.

The following are **out of scope**: social engineering, physical attacks,
denial-of-service, spam, and testing of systems that do not belong to Noru.

Thank you for helping keep Noru and our users safe.
