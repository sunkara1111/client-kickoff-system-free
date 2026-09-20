# Client Kickoff System

**Inquiry to first kickoff in 24 hours — Notion OS + AI prompt engine for solo freelancers**

**Price:** Free  
**Format:** Paste into Notion (or any notes app) · PDF-ready guide · Shareable structure  
**License:** Personal Use License for your freelance business (see `LICENSE-Personal-Use.txt`)

**Created by [Dineshgopi Sunkara](https://github.com/sunkara1111)**  
Senior Controls Engineer · Automation Engineer

---

## What this is

A complete client onboarding system you can run in Notion (or paste into Docs/Notes). It turns a new inquiry into a scheduled kickoff—with intake, scope, welcome packet, payment checklist, and AI prompts—so you stop reinventing onboarding every time.

**Outcome:** Inquiry → first kickoff call within 24 hours (when the client responds promptly).

---

## A. How to use (duplicate into Notion)

### One-time setup (~20 minutes)

1. Create a new Notion page titled **Client Kickoff System**.
2. Create a child page or database for **Client Pipeline** using the schema in Section B.
3. Create a folder/page called **Templates** and paste each template from Section C as its own page.
4. Create a page called **AI Prompt Engine** and paste Section D.
5. Duplicate the **Sample Client: Acme Brand Refresh** (Section E) once so you can see a filled example; keep the blank templates separately.
6. Optional: Add a Notion button or simple checklist page for the **20-minute setup checklist** (Section F)—or just follow it once.

### For every new client (repeatable flow)

1. New inquiry arrives (email, DM, form).
2. Add a row in **Client Pipeline** → status `Inquiry`.
3. Run **Prompt 1: Inquiry Reply** → send.
4. If interested → set status `Qualified` → send **Welcome Email** + **Info Request** (Prompts 2–3) and share/duplicate the **Client Intake** questionnaire.
5. When intake returns → draft **Scope of Work** (use template + Prompt 4) → status `Scope Sent`.
6. On approval → send invoice (use **Invoice & Payment Checklist**) → status `Payment Pending`.
7. On payment (or deposit) → schedule kickoff (Prompt 5) → status `Kickoff Scheduled` → run **Kickoff Call Agenda**.
8. After kickoff → status `Active` → use **Revision Tracker** rules during delivery.
9. Mid-project → optional **First-Week Check-in** (Prompt 7).
10. When done → **Project Handoff / Close-out** → status `Completed`.
11. If not a fit at any early stage → Prompt 6 (decline) → status `Declined` or `Not a Fit`.
12. If scope expands mid-project → Prompt 8 (soft pushback) → update Scope / Pipeline notes.

### Notion duplication tip

- Duplicate the whole **Client Kickoff System** page for a second service line if needed.
- Or duplicate only the **Templates** page into each new client page so every client gets a fresh Welcome Packet, Intake, Scope, etc.
- Recommended: one Pipeline database for all clients; one set of master templates; duplicate templates *into* each client’s workspace page when they convert.

### If you do not use Notion

Paste the same Markdown into Google Docs, Craft, Obsidian, or Apple Notes. The Pipeline can be a simple table or spreadsheet with the same columns.

---

## B. Client Pipeline database schema

Create a Notion **Database** (table) named **Client Pipeline**.

### Properties (fields)

| Property | Type | Options / notes |
|----------|------|-----------------|
| **Client Name** | Title | e.g. Acme Co — Brand Refresh |
| **Contact Name** | Text | Primary person |
| **Email** | Email | |
| **Channel** | Select | Email, Instagram DM, LinkedIn, Referral, Website Form, Other |
| **Service Type** | Select | Writing, Design, Dev, Consulting, Coaching, Other |
| **Status** | Select | See statuses below |
| **Inquiry Date** | Date | When they first reached out |
| **Kickoff Date** | Date | Scheduled call |
| **Deposit / Amount** | Number | Currency format |
| **Paid?** | Checkbox | |
| **Priority** | Select | Hot, Warm, Cold |
| **Fit Score** | Select | Strong Fit, Maybe, Weak Fit |
| **Next Action** | Text | One concrete next step |
| **Next Action Due** | Date | |
| **Notes** | Text | Short log |
| **Client Page** | URL or Relation | Link to their folder/page with templates |

### Statuses (use exactly these for views)

1. `Inquiry` — raw inbound, not yet replied  
2. `Qualified` — replied; waiting on intake / interest confirmed  
3. `Intake Received` — questionnaire back  
4. `Scope Sent` — SOW out for approval  
5. `Payment Pending` — approved; awaiting deposit/invoice  
6. `Kickoff Scheduled` — paid (or agreed terms); call booked  
7. `Active` — project in progress  
8. `On Hold` — paused by client or you  
9. `Completed` — handed off / closed  
10. `Not a Fit` — declined politely  
11. `Ghosted` — no reply after 2 follow-ups (archive later)

### Recommended views

1. **Today / Next Actions** — Filter: Status is not Completed, Not a Fit, Ghosted; Sort by Next Action Due ascending.  
2. **Pipeline Kanban** — Board grouped by Status.  
3. **Needs Reply** — Status = Inquiry OR (Next Action contains “reply” / “follow up”).  
4. **Kickoffs This Week** — Kickoff Date is within one week.  
5. **Unpaid** — Paid? = unchecked AND Status is Payment Pending or Kickoff Scheduled or Active.  
6. **Active Projects** — Status = Active.  
7. **Archive** — Status is Completed, Not a Fit, or Ghosted.

### Pipeline hygiene rules

- Every row must have a **Next Action** and **Next Action Due**.  
- After you send anything, update Next Action to the client’s expected move (e.g. “Wait for intake — nudge Friday”).  
- Move to `Ghosted` after two polite follow-ups with no reply (space them 3–5 business days apart).

---

## C. Full page templates (real copy)

Duplicate these into Notion as separate template pages. Replace bracketed items with your details.

---

### C1. Welcome Packet

**Page title:** Welcome — Working with [Your Name / Studio]

---

Hi [Client First Name],

Welcome. I’m glad we’re exploring this together. This short packet explains how we’ll work so kickoff is fast and clear.

#### Who I help
I work with [ideal clients — e.g. founders and small teams] who need [outcome — e.g. clear brand visuals / reliable web builds / weekly content] without endless back-and-forth.

#### What you can expect
- **Response time:** Within 1 business day on active projects (Mon–Fri).  
- **Single source of truth:** We’ll keep scope, files, and decisions in [Notion / shared folder / email thread — pick one].  
- **One primary contact:** Please nominate one decision-maker on your side for approvals.  
- **Clear scope:** We agree deliverables and rounds *before* heavy work starts.

#### How projects usually run
1. Intake questionnaire (you)  
2. Scope of Work + quote (me)  
3. Deposit / invoice (you)  
4. Kickoff call (both)  
5. Drafts → revisions (within agreed rounds)  
6. Final delivery + handoff

#### What I need from you for a fast start
- Completed intake (link below)  
- Any existing brand assets, examples, or constraints  
- Preferred kickoff windows in the next 5 business days  

#### Boundaries (so we both stay sane)
- Revision rounds are defined in the Scope of Work. Extra rounds = new estimate.  
- Feedback should be consolidated (one message per round, not drip comments).  
- If priorities change mid-project, we’ll pause and re-scope before continuing.

#### Next step
Complete the **Client Intake** form. Once I have it, I’ll send a Scope of Work within one business day.

Looking forward to building something excellent with you,  
[Your Name]  
[Email] · [Website] · [Timezone]

---

### C2. Client Intake questionnaire (all questions)

**Page title:** Client Intake — [Client / Project Name]

**Instructions for client:** Please answer in writing. Bullets are fine. Incomplete answers slow kickoff.

#### 1. Basics
1. Company / brand name:  
2. Your name & role:  
3. Best email & phone (optional):  
4. Website / social links:  
5. Timezone & typical reply hours:  

#### 2. Project snapshot
6. In one sentence, what do you want delivered?  
7. Why now? What changed or deadline is driving this?  
8. Hard deadline (if any) and why it’s hard:  
9. Soft preferences for timeline:  
10. Budget range (or “need a proposal first”):  

#### 3. Success & audience
11. Who is the end audience / user?  
12. What does “success” look like 30–90 days after delivery? (metrics or feelings OK)  
13. What would make this project a failure?  

#### 4. Inputs & constraints
14. Must-have deliverables (list):  
15. Nice-to-haves (list):  
16. Out of scope / explicitly not included (if known):  
17. Brand guidelines, assets, or references (links or “I’ll attach”):  
18. Technical constraints (platforms, tools, CMS, integrations):  
19. Legal / compliance / accessibility requirements:  
20. Stakeholders who must approve work (names + roles):  

#### 5. Collaboration
21. Preferred tools (Slack, email, Notion, etc.):  
22. Meeting preference: async only / short weekly / kickoff + milestones:  
23. How do you usually give feedback?  
24. Any past freelancers/agencies—what worked or didn’t?  

#### 6. Decision & logistics
25. Who signs off on scope and invoices?  
26. Preferred payment method (if you have one):  
27. Anything else I should know before scoping?

**Thank you.** Reply with this completed page or form. I’ll confirm receipt within one business day and send a Scope of Work next.

---

### C3. Scope of Work template

**Page title:** Scope of Work — [Project Name]  
**Version:** 1.0 · **Date:** [YYYY-MM-DD]  
**Prepared for:** [Client] · **Prepared by:** [You]

#### 1. Objective
[1–3 sentences: the business/creative outcome.]

#### 2. Deliverables
| # | Deliverable | Format / notes | Due (est.) |
|---|-------------|----------------|------------|
| 1 | | | |
| 2 | | | |
| 3 | | | |

#### 3. Process & milestones
1. Kickoff  
2. [Milestone A — e.g. first draft]  
3. [Milestone B — e.g. revisions]  
4. Final delivery / handoff  

#### 4. Revision policy
- Included rounds: **[e.g. 2]** rounds of revisions on [deliverables].  
- A “round” = one consolidated batch of feedback.  
- Additional rounds or new concepts: billed at **[rate]** or quoted separately.  
- Feedback window: **[e.g. 5 business days]** per round; delays may shift timeline.

#### 5. Client responsibilities
- Timely feedback and asset delivery  
- Single decision-maker for approvals  
- Payment per schedule below  

#### 6. Timeline
- Kickoff target: **[date / within X days of deposit]**  
- Estimated completion: **[date or range]**  
- Dependencies: [assets, access, third parties]

#### 7. Investment
| Item | Amount |
|------|--------|
| Project fee | $[X] |
| Deposit (due to start) | $[X] ([Y]%) |
| Final payment | $[X] (due [on delivery / date]) |

Optional add-ons: [list]

#### 8. What’s not included
- [e.g. ongoing retainers, stock licenses, paid ads spend, extra page templates, source file transfers beyond agreed formats]

#### 9. Acceptance
Reply “Approved” to this Scope (or sign below) and pay the deposit to lock the kickoff slot.

**Client approval:** _________________ Date: _______  
**Provider:** _________________ Date: _______

---

### C4. Kickoff Call Agenda (30–45 minutes)

**Page title:** Kickoff Agenda — [Project Name]  
**Date/time:** [ ] · **Attendees:** [ ]

#### Pre-call (you)
- [ ] Scope approved & deposit received (or terms agreed)  
- [ ] Intake reviewed; open questions listed  
- [ ] Shared folder / Notion client page ready  
- [ ] Recording/notes plan set  

#### Agenda
1. **Welcome & roles** (3 min) — who decides what  
2. **Success definition** (5 min) — confirm from intake; refine  
3. **Deliverables walkthrough** (7 min) — what’s in / out  
4. **Timeline & milestones** (5 min) — dates, dependencies  
5. **Assets & access** (5 min) — logins, brand files, examples  
6. **Communication rules** (5 min) — channel, response times, feedback rounds  
7. **Risks & open questions** (5 min)  
8. **Immediate next actions** (5 min) — owner + due date for each  

#### Scripted opener (optional)
“Thanks for joining. Goal today: align on success, confirm scope, and leave with clear next actions so we can move fast this week.”

#### End-of-call checklist
- [ ] Next deliverable and owner confirmed  
- [ ] Feedback channel confirmed  
- [ ] Next meeting or async check-in set (if any)  
- [ ] Notes sent within 24 hours  

#### Post-call note template
**Decisions:** …  
**Open questions:** …  
**Your action items:** …  
**My action items:** …  
**Next check-in:** …

---

### C5. Revision Tracker rules

**Page title:** Revision Tracker — Rules & Log

#### Rules (share with client once)
1. Revisions happen in **rounds**, not continuous chat edits.  
2. Each round: client sends **one consolidated message** (or commented file).  
3. You implement that round, then request the next review.  
4. Included rounds are listed in the Scope of Work.  
5. Mid-round “quick tweaks” that change direction count as part of the current round *or* start a new round—your call; note it.  
6. New features / pages / concepts not in scope = **change request** (re-quote), not a free revision.  
7. Log every round below so nobody argues from memory.

#### Log table

| Round # | Date received | Summary of feedback | Due back | Status | Notes |
|---------|---------------|---------------------|----------|--------|-------|
| 1 | | | | Open / Done | |
| 2 | | | | | |
| Extra | | | | Billable? | |

#### Soft language when rounds are used up
“We’ve used the two included rounds. Happy to keep going—next round is $[X] or we can quote a small add-on. Want me to send options?”

---

### C6. Invoice & Payment Checklist

**Page title:** Invoice & Payment Checklist — [Client]

#### Before sending invoice
- [ ] Scope approved in writing  
- [ ] Amount, currency, and line items match Scope  
- [ ] Deposit % and final payment terms clear  
- [ ] Payment links/methods tested (Stripe, PayPal, bank, etc.)  
- [ ] Invoice number & due date set  
- [ ] Late fee / pause policy stated (if you use one)

#### Invoice email blurb (copy-paste)
Subject: Invoice [##] — [Project Name] — Due [Date]

Hi [Name],  
Attached / linked is invoice [##] for **[Project]** per our approved Scope.  
**Amount due now:** $[X] (deposit / full).  
**Pay here:** [link]  
Kickoff is held for **[date window]** once payment clears.  
Questions? Just reply.  
— [You]

#### After sending
- [ ] Pipeline → `Payment Pending`; Next Action = “Confirm payment”  
- [ ] Calendar reminder +2 and +5 business days if unpaid  
- [ ] On payment → checkbox Paid?; move to `Kickoff Scheduled`; send scheduling link or Prompt 5  

#### If payment is late (day 5–7)
“Friendly nudge on invoice [##]. Happy to adjust the kickoff date if timing shifted—want me to resend the link?”

#### Policies you may include (edit to taste)
- Work starts after deposit clears.  
- Final files release after final payment.  
- Projects pause after [X] days overdue.

---

### C7. Project Handoff / Close-out page

**Page title:** Handoff & Close-out — [Project Name]  
**Date:** [ ]

#### Deliverables checklist
- [ ] All scoped deliverables completed  
- [ ] Final files exported in agreed formats  
- [ ] Source files (if included) packaged  
- [ ] Links / live URLs verified  
- [ ] Credentials transferred or removed as appropriate  

#### Handoff package contents
1. Final deliverables (links/folder)  
2. Short “how to use / edit” notes  
3. Outstanding recommendations (optional next phase)  
4. Invoice status (paid in full?)  
5. Testimonial / referral ask (optional)

#### Close-out email (copy-paste)
Subject: Project complete — [Project Name] handoff

Hi [Name],  
You’re all set. Here’s your handoff package:  
- Files: [link]  
- Notes: [link or bullets]  
- Anything still open: [none / list]  

If you’d like a short Loom walkthrough or a phase-2 proposal, say the word.  
If you were happy with the process, a 2–3 sentence testimonial helps a lot—happy to draft a starter for you to edit.

Thanks for trusting me with this.  
— [You]

#### Internal close-out
- [ ] Pipeline → `Completed`  
- [ ] Archive client page  
- [ ] Record final revenue / time spent (for your rates)  
- [ ] Note what to improve in templates  

---

## D. AI Prompt Engine (8 copy-paste prompts)

**How to use:** Paste into ChatGPT, Claude, or similar. Replace `{placeholders}`. Edit the output to match your voice before sending. Never send AI text without a human pass.

---

### Prompt 1 — Inquiry Reply

**Purpose:** Fast, warm first reply that qualifies and points to next step without underpricing yourself.

**Exact prompt:**
```
You are a professional freelance {service_type} helping me reply to a new client inquiry. Write a concise, friendly email (120–180 words) that: (1) thanks them, (2) mirrors their goal in one sentence, (3) states what I need next (intake or 3 clarifying questions), (4) sets expectation that I'll send a clear scope/timeline after details, (5) does not give a firm price yet. Tone: confident, warm, no hype. My name: {my_name}. Their name: {client_name}. Their inquiry: """{inquiry_text}""". My typical services: {services_summary}. Timezone: {timezone}.
```

**Worked example:**
- `{service_type}` = brand designer  
- `{my_name}` = Jordan Lee  
- `{client_name}` = Sam Rivera  
- `{inquiry_text}` = “Need a logo and basic brand kit for our coffee roastery relaunch in October. Saw your work on Instagram.”  
- `{services_summary}` = logo systems, brand kits, packaging direction  
- `{timezone}` = US Eastern  

**Example output (edit before send):**
> Hi Sam,  
> Thanks for reaching out—and for the kind note about the Instagram work. A logo + basic brand kit for your coffee roastery relaunch in October sounds like a focused, exciting project.  
> To put together a clear scope and timeline, I’ll need a few details (goals, must-haves, references, and budget range). I can send a short intake form, or you can reply with answers to three questions: (1) What must ship before October? (2) Do you need packaging direction or logo/kit only? (3) Who approves the final direction?  
> Once I have that, I’ll follow up with a simple Scope of Work—no fluff.  
> Best,  
> Jordan Lee (US Eastern)

---

### Prompt 2 — Welcome Email

**Purpose:** After they engage; deliver Welcome Packet energy in email form and drive intake completion.

**Exact prompt:**
```
Write a welcome email from {my_name}, a solo {service_type}, to {client_name} at {company}. Goal: make them feel taken care of and get the intake completed within 24–48 hours. Include: brief welcome, how we work (3 bullets), link placeholder for intake {intake_link}, what happens after intake, and response-time expectation. 150–220 words. Tone: professional, human, calm.
```

**Worked example:**
- `{my_name}` = Jordan Lee · `{service_type}` = brand designer · `{client_name}` = Sam · `{company}` = Acme Roastery · `{intake_link}` = https://notion.so/intake-acme  

**Example output:**
> Hi Sam,  
> Welcome—I’m glad we’re getting Acme Roastery’s relaunch organized the right way.  
> How we’ll work:  
> • One clear scope before heavy design starts  
> • Consolidated feedback rounds (no endless chat edits)  
> • Kickoff within about a day of approved scope + deposit  
> Please complete this short intake when you can: https://notion.so/intake-acme  
> When it’s back, I’ll send a Scope of Work within one business day so we can lock timeline for October. I reply within one business day on active threads.  
> Talk soon,  
> Jordan

---

### Prompt 3 — Info Request

**Purpose:** Chase missing details without sounding annoyed.

**Exact prompt:**
```
Draft a polite follow-up asking {client_name} for missing intake info. Missing items: {missing_items}. Project: {project_name}. Keep under 120 words. Offer two options: reply in-line OR finish the intake link {intake_link}. Mention that scope/timeline is blocked on these answers. Tone: helpful, not passive-aggressive.
```

**Worked example:**
- Missing: budget range, hard deadline, approval stakeholders  
- Project: Acme Brand Refresh  

**Example output:**
> Hi Sam,  
> Quick nudge—I can draft Acme’s Brand Refresh scope as soon as I have: (1) budget range, (2) hard deadline for October, and (3) who gives final approval.  
> Easiest path: finish the intake (https://notion.so/intake-acme) or reply with those three bullets. Once they’re in, I’ll turn around a clear Scope of Work.  
> Thanks,  
> Jordan

---

### Prompt 4 — Scope Confirmation

**Purpose:** Turn intake notes into a client-facing scope confirmation email (or intro to the SOW).

**Exact prompt:**
```
Using these intake notes, write a scope confirmation email that summarizes objective, deliverables, revision rounds, timeline, price, and deposit. Ask them to reply "Approved" or list changes. Intake notes: """{intake_notes}""". Price: {price}. Deposit: {deposit}. Revision rounds: {rounds}. Timeline: {timeline}. My name: {my_name}. Client: {client_name}. Keep structured with short bullets. No legal jargon.
```

**Worked example:**
- Price $2,400 · Deposit $1,200 · 2 rounds · Timeline kickoff next week, finals in 3 weeks  
- Notes: logo + brand kit (colors, type, usage); no packaging; October soft launch  

**Example output:**
> Hi Sam,  
> Here’s the scope for Acme Brand Refresh based on your intake—please reply **Approved** or send edits.  
> **Objective:** Logo + basic brand kit for October soft launch (no packaging in this phase).  
> **Deliverables:** Primary logo, simplified mark, color palette, type recommendations, one-page usage guide (PDF).  
> **Revisions:** 2 consolidated rounds.  
> **Timeline:** Kickoff within 3 business days of deposit; target finals ~3 weeks after kickoff (depends on feedback speed).  
> **Investment:** $2,400 · Deposit $1,200 to start · Remainder on delivery.  
> If this matches your expectations, I’ll send the invoice next.  
> — Jordan

---

### Prompt 5 — Kickoff Scheduling

**Purpose:** Book the call fast after payment/approval.

**Exact prompt:**
```
Write a short scheduling email for a {duration}-minute kickoff call with {client_name} for {project_name}. Payment/status: {payment_status}. Offer {scheduling_link} OR three time options in {timezone}: {time_options}. List 3 things they should prepare. Under 140 words. Warm and clear.
```

**Worked example:**
- 45-minute call · Deposit received · Calendly link · Options: Tue 10am, Wed 2pm, Thu 11am ET  

**Example output:**
> Hi Sam,  
> Deposit received—thank you. Let’s do a 45-minute kickoff for Acme Brand Refresh.  
> Grab a slot here: {scheduling_link}  
> Or reply with one of these ET times: Tue 10:00 · Wed 14:00 · Thu 11:00.  
> Please bring: (1) any must-use brand constraints, (2) 3–5 reference links (like/don’t like), (3) who will join for approvals.  
> I’ll send a short agenda once booked.  
> — Jordan

---

### Prompt 6 — Not-a-Fit Decline

**Purpose:** Decline graciously; protect reputation; optional referral.

**Exact prompt:**
```
Write a polite decline to {client_name} for {project_name}. Reason (honest, brief): {reason}. Do not over-apologize. Offer {referral_line_or_none}. Leave door open for a better-fit future project. 90–130 words. Tone: respectful, clear, zero guilt-tripping.
```

**Worked example:**
- Reason: timeline requires full brand system + packaging in 10 days; not feasible at quality bar  
- Referral: “I can intro you to two designers who take rush packaging”  

**Example output:**
> Hi Sam,  
> Thanks for the detail on Acme’s October timeline. I don’t want to take this on knowing a full logo system plus packaging in 10 days would compromise quality—and that’s not fair to you.  
> If helpful, I can introduce you to two designers who handle rush packaging more often.  
> If you later want a focused logo + brand kit with a healthier timeline, I’d be glad to revisit. Either way, I appreciate you reaching out.  
> Best,  
> Jordan

---

### Prompt 7 — First-Week Check-in

**Purpose:** Proactive status after kickoff; reduce anxiety; catch blockers early.

**Exact prompt:**
```
Write a first-week check-in message to {client_name} about {project_name}. Status summary: {status_summary}. Ask one question about {open_question}. Confirm next milestone date {next_milestone}. Keep under 110 words. Tone: calm, competent, collaborative.
```

**Worked example:**
- Status: moodboards + first logo directions in progress  
- Open question: preference between wordmark-heavy vs. icon-forward  
- Next milestone: first concepts Friday  

**Example output:**
> Hi Sam,  
> Quick week-one check-in on Acme Brand Refresh: moodboards are underway and I’m shaping the first logo directions.  
> One question to keep us aligned: are you leaning wordmark-heavy or icon-forward for the soft launch?  
> Next milestone: first concepts Friday. Ping me if anything on your side changed.  
> — Jordan

---

### Prompt 8 — Scope Creep Soft Pushback

**Purpose:** Protect boundaries without damaging the relationship.

**Exact prompt:**
```
A client asked for something outside scope: """{creep_request}""". Original scope summary: """{original_scope}""". Write a short reply that: acknowledges the idea, explains it's outside current scope, offers 2 options (defer to phase 2 OR paid change order with rough {change_order_range}), and invites their preference. Under 130 words. Tone: friendly, firm, solution-oriented. Sign as {my_name}.
```

**Worked example:**
- Creep: “Can we also do packaging for the 12oz bag this round?”  
- Original: logo + brand kit only  
- Range: $800–$1,200  

**Example output:**
> Hi Sam,  
> Love that you’re thinking about the 12oz bag—that’s a smart next layer. Packaging isn’t in our current scope (logo + brand kit only), and I want to do it properly rather than squeeze it in.  
> Two options: (1) keep this phase focused and tackle packaging as phase 2 after the kit lands, or (2) I can send a change order roughly in the $800–$1,200 range to add bag packaging now.  
> Which do you prefer?  
> — Jordan

---

## E. Sample pre-loaded client — “Acme Brand Refresh”

Use this as a filled example. Duplicate, then replace with real clients.

### Pipeline row

| Field | Value |
|-------|--------|
| Client Name | Acme Roastery — Brand Refresh |
| Contact Name | Sam Rivera |
| Email | sam@acmeroastery.example |
| Channel | Instagram DM |
| Service Type | Design |
| Status | Kickoff Scheduled |
| Inquiry Date | 2026-09-10 |
| Kickoff Date | 2026-09-15, 10:00 ET |
| Deposit / Amount | 1200 |
| Paid? | Yes |
| Priority | Hot |
| Fit Score | Strong Fit |
| Next Action | Send kickoff agenda + folder access |
| Next Action Due | 2026-09-14 |
| Notes | October soft launch; no packaging in v1 |

### Welcome (filled excerpt)

Hi Sam,  
Welcome. I’m glad we’re organizing Acme Roastery’s relaunch the right way… *[full Welcome Packet with Jordan Lee details, Eastern timezone, Notion as source of truth]*.

### Intake (filled highlights)

- Deliverable: Logo + basic brand kit  
- Why now: Soft launch October; old logo feels generic  
- Success: Recognizable mark on cups/site; cohesive colors  
- Out of scope: Packaging, full guidelines book, photo art direction  
- Budget: $2,000–$3,000  
- Approver: Sam Rivera (founder)

### Scope (filled highlights)

- Fee $2,400 · Deposit $1,200 · 2 revision rounds  
- Deliverables: primary logo, submark, palette, type recs, 1-page usage PDF  
- Kickoff within 3 business days of deposit; finals ~3 weeks post-kickoff  

### Kickoff agenda (filled)

Attendees: Sam Rivera, Jordan Lee  
Focus: success metrics, reference likes/dislikes, asset handoff, Friday concept date  

### Revision log (empty ready)

Round 1 / 2 rows blank; Extra row noted as billable if used  

### Payment

Invoice #1042 paid 2026-09-12 · Remaining $1,200 due on delivery  

### Handoff (preview — not yet)

Will include final SVG/PNG package, usage PDF, and phase-2 packaging proposal stub  

---

## F. 20-minute setup checklist

Do this once. Check each box.

### Minutes 0–5 — Shell
- [ ] Create Notion page **Client Kickoff System**  
- [ ] Create database **Client Pipeline** with all properties from Section B  
- [ ] Add Kanban view by Status + “Today / Next Actions” view  

### Minutes 5–12 — Templates
- [ ] Create **Templates** subpage  
- [ ] Paste Welcome Packet, Intake, Scope, Kickoff Agenda, Revision Tracker, Invoice Checklist, Handoff (Section C)  
- [ ] Replace `[Your Name]`, email, timezone, payment link placeholders with yours  

### Minutes 12–16 — Prompts
- [ ] Create **AI Prompt Engine** page; paste all 8 prompts  
- [ ] Star/favorite the prompts you use most (Inquiry Reply, Scope Confirmation, Scope Creep)  
- [ ] Test Prompt 1 once with a fake inquiry so you trust the flow  

### Minutes 16–20 — Sample + dry run
- [ ] Duplicate **Acme Brand Refresh** sample into Pipeline + a sample client page  
- [ ] Walk Inquiry → Qualified mentally; note where *your* payment link and calendar link go  
- [ ] Add your calendar link and invoice tool links to Invoice Checklist + Prompt 5  
- [ ] Optional: export this guide to PDF for offline reference  

**You’re live.** Next inquiry: new Pipeline row → Prompt 1 → go.

---

## Quick reference — 24-hour kickoff path

| Hour | Action |
|------|--------|
| 0 | Inquiry in → Pipeline `Inquiry` → Prompt 1 reply |
| 0–2 | They engage → Welcome + Intake (Prompts 2–3) |
| Same day | Intake back → Scope (template + Prompt 4) → `Scope Sent` |
| Same day | Approved → Invoice checklist → `Payment Pending` |
| Same day / next morning | Paid → Prompt 5 schedule → `Kickoff Scheduled` |
| ≤24h from ready client | Kickoff held or firmly booked |

*Requires client responsiveness. Your side should never be the bottleneck.*

---

## License & use notes

- Free personal use for your own freelance/solo practice.  
- Do not resell or republish this product as your own template pack.  
- Editing prompts and templates for your voice is expected and encouraged.

See `LICENSE-Personal-Use.txt` for the complete terms. No patent numbers are claimed for this work.

---

*Client Kickoff System · Inquiry to first kickoff in 24 hours · Created by Dineshgopi Sunkara · Built for solo freelancers*
