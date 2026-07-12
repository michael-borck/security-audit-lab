# Security Audit Lab — Engagement Guide

> Part of the **[Assume-Breach series](https://michael-borck.github.io/security-labs/)** — the
> govern/assure end of the arc. Companion to the book
> **[*Substantiate, Don't Assume*](https://michael-borck.github.io/substantiate-dont-assume/)**.

You are an independent security consultant. **Tessera** — a fictional Australian cloud-services company,
recovering from a data breach — has engaged you to give its board independent assurance that its
**Essential Eight** controls are *real*, not just written down. Your job is to find out, and to
**substantiate** whatever you conclude.

This lab is not a Docker lab. Its two moving parts are both on the web:

- **[Tessera](https://tessera.locoensayo.org)** — the company you audit. It has a
  [policy library](https://tessera.locoensayo.org/docs/policies.html), a
  [Statement of Applicability](https://tessera.locoensayo.org/docs/support/statement_of_applicability.html),
  evidence logs, and a dozen [staff you can interview](https://tessera.locoensayo.org/chatbots/) (AI
  chatbots who answer as their character, redirect you to the right person, and won't do your analysis for you).
- **The [Audit Workbench](https://michael-borck.github.io/security-audit-lab/workbench.html)** — your
  workspace for planning, scoping, recording evidence, and building the report.

## How the engagement runs

1. **Plan.** Open Tessera and get a feel for the business — read a few policies, skim the SoA, see who
   works there. This is your kickoff meeting: understand what the client is worried about before you scope.
2. **Scope.** Choose which of the Essential Eight to assess, and *write down why*. You can't cover
   everything; deciding what matters most for this company, post-breach, is an audit skill in itself.
3. **Fieldwork.** For each control, gather evidence three ways — the auditor's method:
   - **Inspect** a document (a policy, the SoA, a register).
   - **Inquire** of a person (interview the right staff member; corroborate their claims).
   - **Observe** the system (read the logs and evidence).
   The workbench gives you an **evidence room** of *everything* Tessera has. It will **not** tell you
   which items bear on a control — working that out is the audit.
4. **Review.** The workbench gives you feedback on whether you *substantiated* each rating.
5. **Report.** Assemble scope, findings, evidence, recommendations and appendices; export as PDF or Markdown.

## The audit method — and how you're assessed

**There is no single correct verdict.** Two auditors can defensibly rate a control *Partial* vs *Not met*
and both be right — *if* the evidence supports it. What is never defensible is:

- a rating with **no evidence** (an assumption — the one thing an audit can't do);
- a rating from a **single source** you never corroborated (a policy is a *claim*; test it);
- **missing** evidence that was there to be found (you didn't interview the right person, didn't read the
  key log).

So you are assessed on **substantiation, not correctness** — did you gather relevant evidence, corroborate
it across sources, and give a rating you could defend to the client? *A Partial you can defend beats a Met
you can't.* The workbench flags all of this, and shows a **defensible example** per control — one good
answer, explicitly *not* "the" answer.

## Two things to keep straight

- **This is an advisory / self-audit**, not **ISO 27001 certification**. Tessera hired you to find and fix
  gaps; the motive for honesty is reputation and improvement, not a certificate. ISO 27001 certification is
  a formal, accredited, third-party audit with a defined scope and recurring surveillance audits.
- **An audit is a snapshot.** Your findings describe the controls *at the time you tested them* — not a
  warranty they still hold next week. That's why audits recur.

## A note on scope limitations

You have Tessera's documents and its people, but **not access to its endpoints**. So three Essential Eight
controls — application control, Office macro settings, and user application hardening — can only be
*partly* tested: you can inspect the standard and interview the SOE team, but you cannot independently
verify enforcement. Rate what you can, and **record the limitation** — documenting what you couldn't test,
and why, is itself part of a professional audit.

## Going further — Incident Zero

Enjoyed pressure-testing a company's controls? *[Incident Zero](https://incidentzero.retroverse.studio/)*'s
**Audit &amp; Compliance** module plays the same gap-analysis as a cooperative game — its 6-domain PASS/FAIL
mirrors an Essential Eight maturity review. (Free, print-and-play.)

## For facilitators

Model answers, the planted-gap map, and marking guidance are **not** in this public repo — they live in the
private `security-labs-staff` companion. Email the maintainer for access.
