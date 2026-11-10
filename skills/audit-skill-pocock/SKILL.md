---
name: audit-skill-pocock
description: "Audits a skill or agent instructions rule by rule against Matt Pocock's writing-for-agents guidance and Theo's additions, then drafts a refactoring plan. Use when tightening a SKILL.md, AGENTS.md or prompt."
disable-model-invocation: true
---

# Audit skill Pocock

## References

Fetch the latest versions from `main`:

- https://github.com/mattpocock/skills/blob/main/skills/productivity/writing-for-agents/SKILL.md
- https://github.com/mattpocock/skills/blob/main/skills/productivity/writing-for-agents/SKILL-MECHANICS.md

If a reference fails, locate its latest canonical version in Matt Pocock's GitHub repositories. Verify authorship and document identity before using it. Report unresolved references.

## Additions inspired by Theo (t3.gg)

Apply these alongside Matt's rules, only where the target skill has the matching branch:

- **Authority**: a skill that runs irreversible actions (merge, force push, deploy, delete) carries an explicit grant for each, unless always-loaded instructions already give it.
- **Loops**: an iterating or review loop carries a round budget (3; up to 5 for security, permission or data-loss changes), stops early when only nits remain, runs one reviewer at a time and lets the agent push back on unneeded suggestions. Its final note states the outcome, the models used and any unresolved dissent.
- **Smallest change**: a skill that edits code or documents aims for the smallest change that meets the intent.
- **Proof**: done means observed evidence of real behavior: CLI output, a screenshot, a bug reproduced then passing, green CI. A mocked test alone does not count.

## Procedure

1. Identify the attached or discussed skill and its supporting files. Extract every distinct rule from Matt's references and the additions above.

2. For each rule, independently review the entire target skill. Record violations, inefficiencies, and improvement opportunities, each with the quoted passage, the rule it touches and a proposed rewrite. Track satisfied and inapplicable rules.

3. Consolidate findings into complementary improvements. Evaluate their combined effects across all rules, including dependencies, conflicts, and trade-offs. Preserve existing intent, behavior, and user decisions.

4. Decide the scope. Targeted edits are the default. Choose a structural rewrite only when the section order departs from the execution order, one problem runs through so much of the skill that isolated edits would leave it incoherent, or steps and reference lack a clear hierarchy.

5. Present a prioritized audit report with actionable recommendations, the scope decision, and a brief rule-coverage summary. When the skill already meets the rules apart from minor touches, say so plainly and close the audit with the report.

6. Resolve material uncertainties through the native interactive question widget, falling back to chat if unavailable. Request approval to draft a unified refactoring plan.

Draft the plan only after approval, opening a rewrite plan with the new section skeleton. Apply changes only with separate authorization.
