# Contributing

## ALFA Principle

> **You do not exist until you prove you are worth it.**

No contribution is accepted until it proves **source, scope, safety, and value**.

This is not a style guideline. This is the law of the system.

---

## What every contribution must prove

### Source
- Where did the code come from?
- If AI-generated: which model, which prompt, what was reviewed?
- If human-written: who, and with what intent?

Code of unknown origin is not trusted.

### Scope
- What does this change actually touch?
- Does it stay within its stated boundary?
- Does it introduce hidden dependencies or side effects?

Code that touches more than it claims is not trusted.

### Safety
- Does it break existing behavior?
- Does it introduce security vulnerabilities?
- Does it handle errors, edge cases, and failure modes?
- Was it tested?

Code that is untested is not trusted.

### Value
- Does it solve the problem it claims to solve?
- Is it solving a real problem, or a perceived one?
- Does it make the system better, or just different?

Code that does not prove its value is not merged.

---

## Contribution checklist

Before opening a pull request, verify:

- [ ] **Source** — origin of the code is documented (author, model, prompt if AI-assisted)
- [ ] **Scope** — change is limited to what the PR description says
- [ ] **Safety** — existing tests pass, new tests added where applicable, no new vulnerabilities
- [ ] **Value** — the PR description explains what problem is solved and why this solution

Pull requests that do not address all four points will be closed without review.

---

## Anti-vibe-coding rules

- Do not open a PR that "kind of works."
- Do not merge code you do not understand.
- Do not ship generated code that has not been reviewed line by line.
- Do not pass validation by disabling tests.
- Do not describe a PR as "misc fixes" or "cleanup" without specifics.

---

## Commit messages

Use the format:

```
<type>: <short description>

<body explaining what changed, why, and what was tested>
```

Types: `feat`, `fix`, `refactor`, `docs`, `test`, `chore`, `security`

---

## The standard

> Nothing exists until it proves its right to exist.

This repo enforces that standard at every level: commit, PR, release, deployment.
