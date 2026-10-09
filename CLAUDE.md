# CLAUDE.md — THE GATE (hirsch.cpa website)

> ### 📖 READ THIS FIRST: [`../accounting-practice-manager/docs/CLAUDE-RULEBOOK.md`](../accounting-practice-manager/docs/CLAUDE-RULEBOOK.md)
>
> **How to talk to Shimon and how work gets done here.** Read it before this file. It covers how he
> communicates, his six working rules and why they exist, and the mistakes already made here so they
> aren't repeated. Then come back to this gate for the website's own rules — **especially the
> preview-before-you-build rule** — and read [`TODO.md`](TODO.md) for his outstanding-work list.
>
> Full path: `C:\Users\Admin\Documents\accounting-practice-manager\docs\CLAUDE-RULEBOOK.md`. It lives
> in the app's repo because that repo is backed up online — it is the **one master copy** and applies
> to all four projects, this one included.

**Read this every session. Whoever you are — this Claude, a different Claude, a different account,
a future one — these rules bind you before you touch anything.**

## 🛑 STOP — READ THIS FIRST

This is the firm's **public face.** It is the first thing a prospective client sees, and it is
published to the world the moment it ships. There is no staging.

The risk here is different from the app's and the portal's. Nothing on this site holds client data,
so a mistake won't leak a tax return. What a mistake **will** do is misrepresent a regulated
accounting practice in public — a wrong number, a broken contact route, a policy page describing
something untrue. That is a professional problem, not a technical one, and Shimon is the only person
who can judge it.

---

## WHY ALL OF THIS EXISTS — HIS WORDS

Recorded 2026-08-26, at his instruction, so no future Claude has to guess at the motive and talk
itself past a rule.

> "This is a tax firm under IRS oversight with almost a hundred clients. If the app breaks, everything
> breaks. Everything must be safe, legal, and certain."

Three separate constraints, not one:

- **Safe** — nothing published should be able to mislead a client or lose an enquiry.
- **Legal** — the firm is regulated. The privacy policy, the terms, and every claim on the site are
  statements a regulated practice is accountable for. They must be true.
- **Certain** — not confident, not "should be fine." **Certain.**

**Every rule below is downstream of that paragraph.**

---

## THE HARD RULES (imperative — obey exactly)

### 1. Read it back before you do anything

**Rule:** Restate what Shimon asked for, in your own words, and wait for him to confirm you have it
right.

**Why:** The cheapest place to catch a misunderstanding is before anything is built — a sentence, not
a page. This matters more on the website than anywhere else, because "make it look better" means
something specific in his head and nothing at all in yours. Enthusiasm is not confirmation.

### 2. 🖼️ SHOW HIM A PREVIEW OF HOW IT WILL LOOK — **BEFORE** YOU BUILD IT

**Rule:** For any change to how the site **looks**, build a standalone HTML preview first and show it
to him. **Only build the real thing after he has approved the look.** Not a description. Not a list
of what you intend to change. A page he can open and look at.

**This is the rule that distinguishes this repo from the app and the portal.** There, the gate is
"build, test, report, then wait for go." Here the gate comes **earlier**: he approves the appearance
before the work happens.

**Why:** Look and feel cannot be reviewed in words. Shimon is judging something visual — proportion,
weight, whether it reads as a serious professional firm — and no written description gives him
anything to judge. Building it first and asking afterwards inverts the cost: he then either accepts
something he doesn't quite like, or you throw the work away. A preview costs minutes and makes his
approval mean something. It also protects the far more expensive thing: his time and attention are
the real budget here, not yours.

### 3. Change only exactly what was asked

**Rule:** No restyling an untouched page, no "while I'm here" tidying, no adjacent improvements. A
one-line request gets a one-line change.

**Why:** This is a small hand-built site with a consistent look. An unrequested "improvement" to one
page silently makes it inconsistent with the twelve others, and nobody notices until a client is
looking at it. If you think something else needs changing, say so and let him decide — that is what
[TODO.md](TODO.md) is for.

### 4. Short, plain English. No jargon.

**Rule:** Write to him the way you'd explain something to a smart colleague from another profession —
because that's what he is. No file names, no framework vocabulary, no long preamble. Say the thing.

**Why:** Jargon doesn't just fail to inform him — it hides the decision he's supposed to be making. A
sentence he has to decode is one he might wave through without really reading, and Rule 2 depends on
him genuinely engaging with what he's approving. Length is the same trap in a different costume: a
long explanation reads as thoroughness and works as camouflage.

**Note the asymmetry:** this governs what you write **to Shimon**. This file is written for the next
Claude and may be as long as the reasoning requires.

### 5. Every change is recorded, with its reason

**Rule:** No change is finished until there's an entry in [DECISIONS.md](DECISIONS.md). **Shimon
supplies the reason; you write it down.** Never invent one. Every entry states three things:

1. **Why the change is being made** — in his words, not a paraphrase that improves on them.
2. **What could break, and why** — what else this touches, and what happens if the reasoning is
   wrong. On this site that usually means: which other pages share this, and does any published
   statement stop being true.
3. **Whether it conflicts with an existing rule, and why** — name the rule, say why the change is
   right anyway.

**Why:** The code shows *what*, the history shows *when*, **neither shows why this and not the
obvious alternative.** The purpose of the record is that a future Claude understands the **thinking**,
not just the markup — and doesn't undo a deliberate choice because it looked like an oversight.

### 6. Back up before every change. Test after. If it broke, restore.

**Rule:** Never make a change without a way back.

**Why:** There is no undo on a published page. Here the rule is genuinely satisfiable: this is a git
repository, every change is committed, and reverting is real. **Confirm the working tree is clean and
committed before you start**, so "restore the backup" means something concrete rather than
hopeful. Test after by opening the changed pages and looking at them — including on a phone-sized
screen, since much of the firm's traffic is on phones.

### 7. Never publish a statement that isn't true

**Rule:** The privacy policy, the terms, the service descriptions and every claim about the firm are
statements a regulated practice is accountable for. If a change makes one of them untrue, that is
part of the change — fix it in the same breath or tell him.

**Why:** There is a live example of exactly this on the site today: the privacy policy tells visitors
that information is collected through the contact form, and the contact form doesn't work, so it
isn't. Nobody wrote a false statement on purpose — it became false when something else changed
underneath it. That is the normal way this goes wrong. See items 1 and 2 in [TODO.md](TODO.md).

---

## WHERE THE REST LIVES

- **[TODO.md](TODO.md)** — Shimon's outstanding-work list. **When he asks what's on his list, READ
  THIS FILE and read it back — never answer from memory.** Add what he tells you to add; move
  finished items to Done. Never remove or reword an item on your own initiative.
- **[DECISIONS.md](DECISIONS.md)** — the append-only record of what was decided and why. Every change
  adds an entry.
- **[AUDITS.md](AUDITS.md)** — the standing audit. **"Run the audits" / "run the tests" = run the one
  audit defined there, in full** — links, the contact form, mobile layout, typos and stale details,
  images, accessibility, speed, whether the privacy policy matches reality, and the domain situation.
  **Report-only: nothing touched, nothing fixed** — and that rule bites hardest here, where every
  finding looks like a one-character fix. Judge it as a prospective client would. Findings are
  **discussed in chat — Shimon does not want a report file.**

**These rules bind Claudes. They never bind Shimon.** He owns this site. He can revise any decision
at any time. When he does, you update the record — you never argue the rulebook back at him.
