# Security Audit Lab

> **Part of the [Assume-Breach series](https://security.borck.education/)** — five hands-on security labs, two companion books, and a game (this is the **govern / audit** end). Browse them all at the [series hub](https://github.com/michael-borck/security-labs).

Play the **security consultant**: audit the fictional company **[Tessera](https://tessera.locoensayo.org)**
against the **Essential Eight** by reading its policies, interviewing its staff, and gathering evidence —
then rate each control and **substantiate every finding**. There's no single right answer; you're judged on
whether your evidence holds up.

**→ [Start the lab](https://securityaudit.borck.education/)** ·
**[Open the Audit Workbench](https://securityaudit.borck.education/workbench.html)** ·
**[Engagement guide](LAB-GUIDE.md)**

## Not a Docker lab

Unlike its siblings, this lab isn't containers — auditing is a documents-and-judgement discipline, so it's a
web + interview simulation (see the series'
[Why Docker guide](https://github.com/michael-borck/security-labs/blob/main/WHY-DOCKER.md) for why that's
the right tool here). Two parts, both hosted:

- **[Tessera](https://tessera.locoensayo.org)** — the company you audit: a policy library, a Statement of
  Applicability, evidence logs, and a dozen interviewable staff (AI chatbots). *Tessera is a separate,
  reusable simulated organisation; this lab audits it.*
- **The Audit Workbench** (`docs/workbench.html`) — a self-contained page: plan → scope → fieldwork
  (an evidence room of everything Tessera has) → substantiation feedback → report. It records and reasons;
  it never tells you where to look.

## How it teaches audit, not click-through

The workbench deliberately **doesn't** hand you the sources for a control. You choose from the full, noisy
set of Tessera's policies, people and logs — most are irrelevant to any given control, and working out
which matter (and who's worth interviewing) is the skill. Feedback grades your *evidence*, not your verdict.

## What's here

- `docs/index.html` — the landing page (GitHub Pages).
- `docs/workbench.html` — the Audit Workbench app.
- `LAB-GUIDE.md` — the engagement guide.

Answer keys and marking guidance are **not** here — they live in the private `security-labs-staff` repo.

## Licence

MIT. Unit-agnostic teaching material.
