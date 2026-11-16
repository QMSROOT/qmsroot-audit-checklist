# QMSROOT Audit Checklist

Turn your own procedure into an audit checklist you can actually use: tailored, risk-based, with the evidence to sample. Free to use.

**Status: version 0.1.0 (pilot).** Feedback welcome via https://qmsroot.com.

## What it does
- **Quick setup:** tick-box options for standard, audit type, depth and format where your Claude app supports them (a short prose question otherwise), or just say "go" for defaults (ISO 13485, internal audit, standard depth, spreadsheet).
- **Built from your procedure:** upload your SOP and the checklist follows what it actually says, with a section reference on every line. Requirements your SOP does not cover are marked "SOP silent" with a question on how they are met in practice.
- **Procedure pre-check:** notes document status (draft, unapproved, no revision), unassigned roles, missing records and placeholder text, and turns each into a line to verify.
- **Risk-based:** add recent findings, complaints or changes, and the checklist prioritises lines High / Medium / Low with a reason.
- **Evidence, not yes/no:** every line has an open audit question, the records to sample with a suggested sample size and why, and where the audit trail leads next.
- **Ready to fill in:** blank Result (C / NC / OBS / N/A / Not audited) and Notes columns, plus a list of records to request before the audit.
- **Frameworks:** ISO 13485, MDSAP (by jurisdiction), ISO 9001 (edition as you state it), FDA QMSR-style, GMP (by regime), and supplier audits.
- **Source discipline:** requirements are paraphrased; clause numbers appear only when verified or taken from your own copy of the standard.
- **Privacy prompts:** reminds you to anonymise names, suppliers and patient data before every upload.

Pairs with **QMSROOT Mock Auditor**: build the checklist, then practise the audit.

## Installation

### Claude (web, desktop and Cowork)
- **From the Claude directory (once listed):** open **Customize → Plugins → Discover**, search for "QMSROOT Audit Checklist" and add it.
- **Before it is listed:** download this repository as a ZIP (green **Code** button → **Download ZIP**), then in Claude open **Customize → Plugins**, choose to add or upload a plugin, and select the ZIP.

### Claude Code
This plugin is listed in the QMSROOT marketplace:

```bash
claude plugin marketplace add QMSROOT/qmsroot-mock-auditor
claude plugin install qmsroot-audit-checklist@qmsroot
```

### Check it works
Start a new conversation and type `/audit-checklist` or "make me an audit checklist". Claude should ask for the standard, audit type, depth and format.

## What the plugin runs and sends
The plugin contains only instructions and reference text. It runs no scripts, installs no packages, connects to no external services and sends no data anywhere. Documents you upload are handled by Claude like any other conversation content. The checklist is created with whatever spreadsheet or document tool your Claude session already has, or shown in the chat.

## Limitations
- A preparation tool, not an audit, certification decision or regulatory advice. A completed checklist records what was seen; it is not a conformity decision.
- Requirements are paraphrased; check clause numbers and wording against your licensed copy.
- Many framework facts (editions, dates, timelines) are deliberately marked unverified; see `skills/audit-checklist/references/reference-status.md`.
- Anonymise everything you share. Your organisation's AI policy applies.

## Licence
QMSROOT Audit Checklist is © 2026 MAXCERT LTD, trading as QMSROOT, and free to use under the **QMSROOT Free-Use Licence** (see [LICENSE.md](LICENSE.md)). In short:

- **You may** install and use it for free, as an individual, employee, auditor, consultant or commercial organisation, including for internal and supplier audits and while delivering your own paid consulting or training. You may use the checklists you create however you like.
- **You may not** sell it, rebrand it, hand it out as part of a paid product, course or service, or publish modified versions without written permission from QMSROOT.
- **QMSROOT keeps** its copyright and branding; notices and links must stay intact.
- **Preparation tool only:** it is not a certification, audit or regulatory-compliance guarantee.
- **Separately licensed:** the QMSROOT platform, backend intelligence and integrations are not covered by this licence.

The summary is for convenience; [LICENSE.md](LICENSE.md) governs. For permissions or partnerships, contact QMSROOT via https://qmsroot.com.

## Contents
```
.claude-plugin/plugin.json   plugin manifest
skills/audit-checklist/      checklist builder + references
LICENSE.md                   QMSROOT Free-Use Licence
```

---
More at https://qmsroot.com
