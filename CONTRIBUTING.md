# Contributing to UKHO.Abzu.AIEnablement (Documentation / Prompt Repository)

Repository Owner: **Team Abzu**  
Primary Contact: **AbzuDeliveryTeam@UKHO.gov.uk**

This repository currently stores:
- Copilot / AI assistant prompt files (`.github/prompts/*.prompt.md`)
- Governance / usage guidance (e.g. this CONTRIBUTING file, copilot instructions)
- High-level meta documentation only

It intentionally contains:
- No application source code
- No live / authoritative project specifications
- No implementation or refactor execution plans
- No secrets or operational configuration

> By submitting a contribution (prompts, guidance, or meta-docs) you agree it will be released under the repository licence (see: [LICENSE](LICENSE)).

---
## Contents
1. Principles & Ethos
2. Current Scope
3. Ways to Contribute
4. Getting Started
5. Prompt Standards
6. Markdown & Style
7. Review & Pull Requests
8. Accessibility & Inclusive Writing
9. Security & Sensitive Information
10. Licensing
11. Governance
12. Contribution Checklist
13. Future Additions (Planned but Not Yet Present)
14. Questions

---
## 1. Principles & Ethos
- Open-by-default reusable prompt patterns
- Plain English; minimise jargon
- Incremental, reviewable changes
- Traceability: each change must include a concise rationale in the PR description
- Avoid speculative complexity until needed

---
## 2. Current Scope
Included (today):
- Prompt files per family/phase (e.g. `spec.plan.prompt.md`, `refactor.plan.prompt.md`)
- Supporting guidance (Copilot instructions, contribution policy)

Not yet included (future roadmap):
- Formal spec / plan templates (will live under `docs/` when introduced)
- ADR templates
- Versioned template library

Explicitly excluded:
- Live project specs / plans
- Source code, build scripts, infra definitions
- Proprietary or sensitive architectural detail

---
## 3. Ways to Contribute
- Improve clarity, safety, determinism of existing prompts
- Add a new prompt phase (justify purpose in PR rationale)
- Remove duplication or consolidate overlapping guidance
- Tighten instructions to reduce ambiguity / hallucination risk
- Add neutral examples (clearly marked “Example Only”)
- Refine governance or usage notes

Before larger changes (new family / structural reorganisation / deprecation) email: AbzuDeliveryTeam@UKHO.gov.uk OR start a discussion in the PR draft description for alignment.

---
## 4. Getting Started
```
git clone https://github.com/UKHO/UKHO.Abzu.AIEnablement.git
cd UKHO.Abzu.AIEnablement
git checkout -b prompt/<short-slug>
```
Recommended tools:
- markdownlint / cSpell
- Mermaid preview (if adding diagrams)
- Diff viewer with word-wrap

---
## 5. Prompt Standards
File naming: `.github/prompts/{family}.{phase}.prompt.md`
- family examples: `spec`, `refactor`, `test`, `pipeline`
- phase examples: `research`, `plan`, `execute`

Each prompt SHOULD include:
- Role & scope declaration (first lines)
- Clear output contract (code fences or bullet format)
- Constraints / do-nots (to prevent scope drift)
- Completion / termination pattern (if applicable)
- Mandatory phrases required by downstream automation (if any)

Each prompt SHOULD NOT include:
- Project-specific private context
- Secrets, tokens, internal endpoints
- Irreversible or destructive operational instructions

Prompt improvement checklist:
- [ ] Scope statement concise & unambiguous
- [ ] Input/Output expectations explicit
- [ ] No overlapping instructions with another prompt (or justification present)
- [ ] Consistent imperative style
- [ ] Neutral examples marked “Example (Non-Authoritative)"
- [ ] No references to non-existent template files

Versioning: Only add a suffix (e.g. `spec.plan_v1.1.prompt.md`) if a breaking change is required AND automation depends on previous behaviour; otherwise evolve inline.

---
## 6. Markdown & Style
- Single H1 (`#`) per file
- Fenced code blocks with language hints for examples / output formats
- Backticks around file names / literal tokens
- 120 char soft wrap suggested
- Lists focused; avoid deep nesting
- Prefer active voice and imperative instructions

---
## 7. Review & Pull Requests
Branch naming:
- `prompt/<family>-<topic>`
- `docs/<purpose>`
- `governance/<topic>`

PR expectations (include in description):
- Purpose & concise rationale
- Summary of key changes (added / removed directives)
- Any downstream automation impact
- Safety notes (if restricting prior behaviour)

Review focus:
- Clarity & determinism
- Safety (no scope creep / sensitive leakage)
- Consistency (tone, naming, structure)
- Reduction of ambiguity / duplication

---
## 8. Accessibility & Inclusive Writing
- Expand acronyms on first use
- Avoid culture-specific idioms, slang
- Gender-neutral phrasing
- Provide brief captions for diagrams (if added)

---
## 9. Security & Sensitive Information
Do NOT add:
- Internal service names, hostnames, endpoints
- Credentials, keys, access tokens
- Proprietary architecture diagrams
- Live system operational specifics

If uncertain: omit and request guidance via contact email.

---
## 10. Licensing
- MIT licence applies to all contributions
- Attribute external frameworks by name only
- No verbatim proprietary material

---
## 11. Governance
Team Abzu maintains directional coherence:
- May request scope reduction or consolidation
- Encourages additive evolution unless simplification clearly warranted

Escalations / queries: AbzuDeliveryTeam@UKHO.gov.uk

---
## 12. Contribution Checklist
Before marking PR “Ready for Review”:
- [ ] Branch named correctly
- [ ] Rationale included in PR description
- [ ] File naming pattern correct
- [ ] Output contract explicit
- [ ] No sensitive data
- [ ] Examples labelled (if present)
- [ ] Lint / spell checks pass (if configured)
- [ ] Key changes summarised (added / removed)

---
## 13. Future Additions (Not Yet Present)
(Planned – do NOT assume availability; separate changes will introduce these)
- `/docs/specs` (spec templates)
- `/docs/plans` (plan templates)
- `/docs/adr` (decision records) & ADR template
- Formal template versioning policy

---
## 14. Questions
Add question(s) in a draft PR description or email AbzuDeliveryTeam@UKHO.gov.uk with context + desired outcome.

---
Thank you for helping strengthen reusable, safe prompt assets.
