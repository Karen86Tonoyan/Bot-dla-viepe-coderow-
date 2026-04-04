# Security Policy

## ALFA Principle

> *You do not exist until you prove you are worth it.*
>
> No artifact exists outside the sandbox until it proves source, scope, safety, and value.

Security is not an afterthought. It is a gate.

Every artifact in this repository must prove it is **safe** before it exists outside the sandbox. This is not optional and it is not negotiable.

---

## Security Gate

The release pipeline enforces the following security checks. Any artifact that fails is rejected — it does not ship.

| Check | What it validates |
|-------|------------------|
| **Source** | The artifact's origin is known and traceable. No unreviewed external code. |
| **Scope** | The artifact only accesses what it is permitted to access. No scope creep. |
| **Safety** | No known vulnerabilities, no hardcoded secrets, no unsafe dependencies. |
| **Usefulness** | The artifact solves a real, defined problem. No dead code ships. |

---

## Supported Versions

| Version | Supported |
|---------|-----------|
| main branch | ✅ Active |
| older branches | ❌ Not supported |

---

## Reporting a Vulnerability

If you discover a security vulnerability in this repository:

1. **Do not open a public issue.**
2. Open a [GitHub Security Advisory](https://github.com/Karen86Tonoyan/Bot-dla-viepe-coderow-/security/advisories/new) to report it privately.
3. Describe:
   - what the vulnerability is
   - where it was found (file, line, component)
   - how it can be exploited
   - what the impact is
4. We will respond within **5 business days** with an assessment.
5. If the vulnerability is confirmed, a fix will be released and the advisory made public once the fix is in place.

---

## Security Principles

### Nothing is trusted
All input — from users, external APIs, AI models, webhooks — is treated as untrusted by default.  
Validation happens before processing, not after.

### Nothing exists until it proves its right to exist
Generated code, AI output, and external dependencies must be reviewed before they are merged.  
"It works locally" is not a security argument.

### Secrets never enter the repository
- No API keys, tokens, passwords, or credentials in code or configuration files.
- Use environment variables or a secrets manager.
- If a secret is accidentally committed, treat it as compromised immediately and rotate it.

### Dependencies are reviewed
- Every new dependency must be checked for known vulnerabilities before it is added.
- Dependency updates are not automatic — they are reviewed.

### Agents operate within their scope
- No bot or agent may access resources outside its declared scope.
- Scope is defined before the agent runs, not inferred during execution.

---

## Contact

For non-security issues, open a GitHub issue.  
For security issues, use the private advisory process described above.
