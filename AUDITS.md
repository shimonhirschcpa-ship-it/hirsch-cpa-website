# AUDITS — the website's standing audit

**"Run the audits." "Run the audit." "Run the tests."** — on the website, every one of those phrases
means the **same thing, forever: run the single audit defined below, in full, and discuss the findings
with Shimon in chat.** This file exists so that command is **permanent and repeatable** — a fresh
Claude with no memory of the day this was written can open this file and execute it identically.

## Why there is one audit here, not five

The app has [five audits](../accounting-practice-manager/docs/AUDITS.md) and the portal has
[five](../hirsch-portal/docs/AUDITS.md). **This site gets one, deliberately, because it is a different
kind of thing:**

- It is **static pages**. No database, no accounts, no logins, no client data, no scheduled jobs.
- So there is **no engine or clock audit** (it calculates nothing), **no data integrity audit** (it
  stores nothing), and **no connection audit** (it is joined to nothing).
- There is **no security posture or breach audit** in the app's sense — there is no door to test,
  because there is nothing behind one. Security items that *do* apply to a static site are folded into
  section 7 below.

**This is not a lowered bar. It is a different bar.** The whole risk here is **public**: what a
prospective client sees, whether they can reach the firm, and whether everything the site says about
the firm is true. So the audit is Audit B — Design / UI — adapted, broadened, and judged from the
outside.

**If that ever changes, this file changes with it.** In particular: **the moment the contact form
actually starts delivering messages**, the site begins collecting personal information, and a data and
privacy audit becomes warranted. Say so if you find that has happened.

---

## 🛑 THE RULES THAT BIND THIS AUDIT

1. **REPORT-ONLY. Nothing is touched. Nothing is fixed. Ever.** This is Shimon's ironclad rule, in his
   own words: *"Nothing should be touched. Nothing should be fixed. Just check… then send me a
   report… how many tests were wrong."* An audit that finds a broken link **writes it up** — it does
   **not** fix it, not even when the fix is one character. **Fixing is a separate, later
   conversation**, under the normal loop, one approved change at a time. See
   [`CLAUDE.md`](CLAUDE.md) Rules 1 and 3.

   **This bites harder here than anywhere else.** Most findings on this site will be small and
   obviously fixable — a typo, a dead link, a wrong year. The temptation to "just fix it while I'm
   looking" is strongest exactly where the rule matters, because a site-wide sweep of tiny unrequested
   edits is precisely how a consistent site quietly stops being consistent.

2. **Never submit the contact form to a real destination.** If it ever starts working, a test
   submission sends a real message to the firm. Assess it; do not fill it in and send it.

3. **Findings become TRACKED FOLLOW-UPS, not inline fixes.** Anything real goes into
   [`TODO.md`](TODO.md) or is raised with Shimon explicitly.

4. **The audit ends with a PASS/FAIL COUNT and a SEVERITY-RANKED findings list.** "How many were wrong"
   is the deliverable Shimon asked for.

5. **No drifting facts stated as fixed.** State counts as measurements taken on a date, never as
   standing truth.

---

## 🎯 HOW TO JUDGE — read this before you start

**Audit this as a prospective client would see it, not as someone who built it.**

The visitor is a business owner or a taxpayer who needs an accountant. They have probably arrived from
a search or a recommendation, they are comparing two or three firms, and they will decide in under a
minute whether this one looks competent and trustworthy. **They are handing over their tax affairs.**

So the standard is not "does it work." The standard is **"does this look like a professional CPA firm
that I would trust with my finances."** A stale year, a placeholder line nobody removed, a link that
goes nowhere, a page that is unreadable on a phone — each is small on its own and each quietly says
*this firm does not check its work.* That is the wrong message for an accountancy practice to send.

Where something is a judgement call, say so and let Shimon decide. **Do not redesign anything, and do
not report matters of taste as failures.**

---

## THE AUDIT — coverage checklist, walk ALL of it

### 1. Every link resolves

- **Every internal link on every page**, including the navigation, the footer, and links buried in
  body text. Follow each one. A link to a page that does not exist is a FAIL.
- **Every external link** — professional body logos and links, the client portal link, anything
  pointing off-site. Confirm each still goes somewhere real and still goes where it claims.
- **The client login / portal link especially.** This is the one that sends real clients to their real
  tax returns. If it is wrong or dead, that is Critical, not cosmetic.
- **Every email address and telephone number** on the site: correct, current, and clickable where it
  should be.
- **Navigation consistency** — the same menu, in the same order, on every page. Check the services
  pages individually; they are the easiest to leave behind.

### 2. The contact form actually delivers

**This is the highest-value single check on the site.**

- Does the form **actually send anything, anywhere?** Trace it properly. A form that looks complete
  and does nothing is worse than no form — the visitor believes they have contacted the firm and the
  firm never hears from them, with no way to know how many that has been.
- Where does a submission **go**, who receives it, and how would anyone know if it stopped working?
- Does the visitor get a **confirmation** that their message was sent?
- Does the form handle a **failure** visibly, or fail silently?
- Are the fields sensible, labelled, and is anything required that shouldn't be?
- **Known status as of 2026-08-26: it does not work at all** — [`TODO.md`](TODO.md) item 1. Verify
  whether that is still true rather than assuming either way.

### 3. Mobile layout

- **Check every page at 375px.** The HARD rule: **no horizontal overflow, anywhere.**
- Text readable without pinch-zoom; tap targets big enough for a thumb; the menu opens and closes.
- Images scale rather than overflowing or distorting.
- Tables and any wide content reflow rather than forcing the page sideways.
- **Assume a large share of visitors arrive on a phone.** A page that only works on a desktop fails for
  the majority of the people it is meant to persuade.

### 4. Typos, placeholder text, and stale details

- **Read every page's actual words.** Spelling, grammar, punctuation, capitalisation of the firm's own
  name and services.
- **Placeholder text nobody removed** — sample copy, "lorem ipsum", dummy addresses, a stock phone
  number, a heading that was never rewritten.
- **Stale details:** a wrong year in a copyright line, tax deadlines that have passed or belong to a
  previous year, out-of-date filing thresholds, a service the firm no longer offers, or a missing one
  it does.
- **The tax due dates page needs particular care** — it states dates a visitor may rely on. **A wrong
  filing deadline published by a CPA firm is a serious finding, not a typo.** Check it against the
  current year properly.
- **The refund tracking page** — confirm what it tells people is still accurate and still points at a
  working destination.

### 5. Images

- Every image loads; none are broken or missing.
- Sensibly sized — no enormous file being scaled down in the browser, which slows the page badly on a
  phone.
- Every image has meaningful alternative text, for screen readers and for when it fails to load.
- Nothing looks stretched, squashed, or wrongly cropped at any screen size.
- The social sharing preview image works — check what actually appears when a page is shared.

### 6. Accessibility basics

Not a full accessibility review — the basics, which matter both for real visitors and because a
professional firm should meet them:

- Every page reachable and operable **by keyboard alone**; focus is visible.
- **Heading order is sensible** — one main heading per page, no levels skipped.
- **Colour contrast** adequate for body text, buttons and links.
- Form fields **properly labelled** (not placeholder text standing in for a label).
- Each page has a **unique, descriptive title** and a sensible language setting.
- Nothing conveys meaning by colour alone.

### 7. Page speed and the technical basics

- How fast does each page actually load, on a phone-like connection? Oversized images are the usual
  culprit.
- Any errors reported in the browser console; anything failing to load.
- **Security basics that apply to a static site:** the site is served over HTTPS everywhere, no page
  mixes insecure content, and no external script or resource is loaded from somewhere that shouldn't
  be trusted. Note whether standard protective headers are present.
- Confirm nothing sensitive is sitting in the published files — no keys, no internal notes, no
  leftover working files.

### 8. Does the privacy policy match what the site actually does?

- **Read the privacy policy against the site's real behaviour, line by line.** Does the site collect
  what the policy says it collects, and only that?
- **Known contradiction as of 2026-08-26:** the policy tells visitors their information is collected
  through the contact form, and the form does not work, so it isn't — [`TODO.md`](TODO.md) item 2.
  Note that this stops being untrue the moment the form is fixed, and that **fixing the form without
  revisiting the policy would leave the site collecting personal data under a policy nobody rechecked.**
- Does anything else on the site collect data — analytics, embedded content, cookies, external fonts —
  that the policy does not mention?
- Read the terms page the same way: does it describe this firm, this site, and these services
  accurately?
- **Every published claim about the firm must be true.** Professional body memberships, services
  offered, locations, credentials. The firm is regulated and accountable for what it publishes.

### 9. The domain situation

- **What web address is the site actually served from?** Is it the firm's own name, or a temporary
  hosting address?
- Check the "official address of this page" tag on **every** page — the one search engines follow. If
  those point at a temporary address, then moving the site later would leave search engines pointed at
  the old one until each page is corrected.
- Same question for the social sharing tags.
- **Known status as of 2026-08-26:** the site runs on a temporary hosting address and the tags are
  hard-coded to it — [`TODO.md`](TODO.md) item 3. Verify rather than assume.
- **Why this belongs in a design audit:** a visitor about to trust a firm with their tax affairs looks
  at the address bar. An unfamiliar one is exactly what people are taught to be suspicious of. The
  portal has the same gap, and clients are sent there from here.

---

## How to run it

Drive the real site — open every page, follow every link, resize to 375px, read the page structure and
the console, and read the actual words on the page. Where something cannot be checked from here, say
so plainly rather than guessing.

**Report-only.** A dead link is written up, not repaired. A typo is written up, not corrected.

---

## PASS / FAIL

Count what you checked — pages, links, images, form fields, claims — and report it as a count.

**FAIL** = a dead link, a form that does not deliver, horizontal overflow at 375px, a broken or missing
image, a published statement that is untrue, a wrong tax date, placeholder text still visible, or a
page unusable by keyboard.

**PASS with a note** = a judgement call, a matter of taste, or a known trade-off already recorded on
[`TODO.md`](TODO.md).

Severity, for ranking the findings:

- **🔴 Critical** — the portal link is broken or wrong; the site publishes a wrong tax deadline; a
  claim about the firm is untrue; the site is unreachable or insecure.
- **🟠 High** — the contact form does not deliver; a main page is broken on phones; the privacy policy
  contradicts what the site does.
- **🟡 Medium** — a dead internal link, a broken image, a stale year, a real typo in prominent copy.
- **⚪ Low / Note** — cosmetic, a minor wording preference, or an accepted trade-off restated.

---

## When this runs

**On request. There is no fixed schedule.** Shimon asks, and this audit runs.

Worth running additionally: **after any change to the site**, and **at the start of a filing season**,
when the tax dates and deadlines on the site need to be right for the new year.

---

## The findings — discussed in chat, NOT written to a file

**Shimon does not want an audit report file.** He wants the findings **discussed with him in the
conversation.** Do not write a report document, do not save one to `outputs/`, and do not offer one
unless he asks.

Present them the way he reads best — the way
[the rulebook](../accounting-practice-manager/docs/CLAUDE-RULEBOOK.md) describes:

1. **Lead with the answer.** Is the site in good shape, yes or no. First sentence.
2. **The count:** `WEBSITE AUDIT — PASS n / FAIL m`, and what n + m counted.
3. **Findings, most serious first**, using the severity ranking above. For each: what is wrong, which
   page, and what a visitor would experience.
4. **Say plainly what you could NOT check**, and why.
5. **Plain English throughout.** No file names or technical vocabulary unless he asks. Describe what a
   visitor sees, not what the markup does. He is a CPA, not a developer.

**Then STOP.** The audit's job ends at the conversation. Anything that follows is a **separate change**
— and on this site that means the preview rule applies: **anything affecting how a page looks gets an
HTML preview approved before it is built** ([`CLAUDE.md`](CLAUDE.md) Rule 2). Real findings are added
to [`TODO.md`](TODO.md) so they are not lost.

---

> **This is Shimon's decision. No Claude may change it on its own initiative. Only Shimon can revise
> it — and if he does, update this file in the same breath.**
