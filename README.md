# Email Drafting and Review

A reusable skill for concise external business emails, adapted from a personal drafting workflow.

## 中文说明

用于起草、精简、润色和审阅对外英文商务邮件。保留简洁、直接、礼貌及商业和法律表达准确的风格；审阅已有草稿时优先做最小修改。

## Files

- [SKILL.md](SKILL.md): drafting and review.
- [Style profile](references/style-profile.md): reusable writing defaults.
- [Fictional examples](references/examples.md): routine request, structured proposal, and a review boundary.
- [Agent metadata](agents/openai.yaml): display name and invocation prompt.

## Use

Place this repository's contents in a skill directory named `draft-external-email` in your agent's configured skills location. The entrypoint is `SKILL.md`; keep `references/` and `agents/` beside it. 

Example requests:

- `Use $draft-external-email to draft a short reply using the facts below.`
- `Use $draft-external-email to review this email. Preserve my structure and flag changes to commitments.`

The skill produces drafts; sending requires a separate user instruction.

---

## Complete skill instructions

# Draft External Email

Write concise, commercially clear emails: courteous without ceremony and precise without sounding like a legal memo.

## Style context

Read [references/style-profile.md](references/style-profile.md) before drafting or reviewing. Read [references/examples.md](references/examples.md) when a routine request or multi-issue proposal would benefit from an illustration.

Current user instructions take priority over the defaults.

## Draft or revise

1. Identify the recipient, objective, supplied facts, requested action, and any sensitive commercial position. Ask only for missing information that would materially change the message; use clear placeholders for minor missing facts.
2. Use the lightest structure that carries the substance: short paragraphs for routine emails; use short sentences, each containing only one subject; numbered descriptive headings for separate issues in a complex explanation or proposal.
3. Open with acknowledgement or purpose. Include only the background needed for the recipient to understand and act.
4. Use plain business English. Preserve meaningful qualifications, defined terms, exact figures, responsibility, timing, and distinctions between a proposal and an agreed commitment. Ground statements in the supplied facts.
5. Preserve intentional, truthful strategic ambiguity. A proposed process can convey an assumed next step without adding an unsupported express rights claim. Flag ambiguity when it risks changing a commitment or misleading the recipient.
6. End with a concrete invitation to confirm, advise, review, or discuss. Use `Dear [Name],` and `Regards,` where appropriate; use the user's supplied `[Your name]`.
7. Return one recommended version unless alternatives are requested. Include a subject when requested or useful.

## Review an existing draft

Preserve its structure and usable wording. Make the smallest edits needed for natural English, precision, concision, and tone. Make sure there is no mistake in grammar. Keep characteristic phrases when they work. Briefly flag edits that materially change legal or commercial meaning, especially obligations, admissions, deadlines, and settlement language.
