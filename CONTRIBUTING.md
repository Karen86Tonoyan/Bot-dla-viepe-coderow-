# Contributing

## ALFA Principle

> *You do not exist until you prove you are worth it.*
>
> No artifact exists outside the sandbox until it proves source, scope, safety, and value.

Every contribution must demonstrate:

| Property | Question to answer |
|----------|--------------------|
| **Source** | Where did this come from? Is it original, reviewed, and traceable? |
| **Scope** | What is it responsible for? Does it stay within its defined boundaries? |
| **Safety** | Does it introduce risk — security, reliability, or correctness risk? |
| **Usefulness** | Does it deliver value? Does it solve a real, defined problem? |

A contribution that cannot answer all four questions **does not pass**.

---

## Rules

### Code does not pass without proof
- All changes must include a clear description of what they change and why.
- Changes that touch security-sensitive areas require explicit review.
- Generated code must be reviewed and understood — generation is not proof.

### Agent does not act without scope
- Every bot action must be bounded by a defined task.
- No agent may perform actions outside its declared scope.
- Scope must be stated before work begins, not after.

### Artifact does not leave without validation
- Nothing is merged without passing the release gate.
- The release gate checks: source, scope, safety, usefulness.
- Failing the gate means the artifact does not exist — it goes back to the sandbox.

### Result does not exist just because it was generated
- AI-generated output is a draft, not a result.
- Every generated artifact must be reviewed, tested, and explicitly accepted.
- "It was generated" is not a reason to ship it.

---

## How to Contribute

1. Fork the repository.
2. Create a branch with a descriptive name: `feature/idea-intake`, `fix/model-router-null`, etc.
3. Make your changes. Answer the four ALFA questions for your change.
4. Open a pull request with:
   - what you changed
   - why it is needed
   - how it was tested
   - which ALFA properties it satisfies
5. Wait for review. The pipeline will run the release gate automatically.

---

## Commit Style

Use clear, imperative commit messages:
- `add task breakdown module`
- `fix missing validation in repo brain`
- `remove unused model router fallback`

Do not write:
- `fix stuff`
- `update`
- `wip`

---

## Questions

If you are unsure whether your change fits the scope of this project, open an issue and describe what you want to do before writing code.
