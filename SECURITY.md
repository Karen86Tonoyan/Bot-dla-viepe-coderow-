# Security Policy

## ALFA Principle

> **No artifact exists outside the sandbox until it proves source, scope, safety, and value.**

Security is not a checklist. It is the proof of existence.

Code that cannot prove it is safe does not leave the sandbox. Period.

---

## Supported versions

| Version | Supported |
|---------|-----------|
| main    | ✅        |
| < main  | ❌        |

Only the current `main` branch receives security fixes.

---

## Reporting a vulnerability

Do not open a public issue for security vulnerabilities.

Report vulnerabilities by emailing the repository owner directly, or by opening a private security advisory via GitHub:

**GitHub Security Advisories:** [Report a vulnerability](../../security/advisories/new)

Include in your report:
- Description of the vulnerability
- Steps to reproduce
- Affected component(s)
- Potential impact
- Suggested fix, if known

You will receive acknowledgment within 72 hours.

---

## Security requirements under the ALFA Principle

Every artifact in this repository must prove:

### Source
- All dependencies must have a verified, auditable origin.
- AI-generated code must be reviewed and signed off by a human before it touches production.
- No code from unknown or unverified sources is accepted.

### Scope
- Every component must operate within a declared, minimal scope.
- No component may access resources, credentials, or data beyond what it explicitly needs.
- Principle of least privilege is mandatory, not optional.

### Safety
- All inputs must be validated before processing.
- All external integrations must be sandboxed before trust is established.
- Secrets must never be committed to source control.
- Dependencies must be pinned and audited.
- No artifact is deployed without passing security checks in CI.

### Value
- Security controls must not be bypassed "just for testing."
- A feature that cannot be secured is not shipped.
- Risk accepted consciously must be documented.

---

## Release gate

No artifact exits the pipeline to production without passing:

1. Automated security scan (SAST)
2. Dependency vulnerability audit
3. Human review sign-off
4. ALFA checklist verification: source ✅ scope ✅ safety ✅ value ✅

If any gate fails, the artifact does not exist outside the sandbox.

---

## Known security posture

- Secrets management: environment variables only, never in source
- Third-party model APIs: scoped tokens, rotated regularly
- Bot permissions: minimum required per integration
- Repository: branch protections enforced on `main`

---

> **You do not exist until you prove you are worth it.**  
> Security is how that proof is made.
