# TO-DO LIST — hirsch.cpa website

**What this file is.** Shimon's running list of outstanding work on the firm's public website. It
lives here, on disk, on purpose: Claude gets reset, updated and replaced, and anything held only in a
chat window disappears when that happens. This file does not.

**How Claude must use it — this is binding:**

1. **When Shimon asks what's on his list, read this file and read it back.** Don't answer from
   memory. Don't answer from a chat further up. Open the file.
2. **When Shimon says to add something, add it here**, in the Open section, with today's date, in
   plain English.
3. **🔁 WHEN SOMETHING SHIPS, CLOSE IT IN THE SAME PASS — DO NOT WAIT TO BE ASKED.**
   *Standing rule, added 2026-09-02. In his words: "Whenever we do something, it should be
   automatically marked down. I don't have to tell you every time. It should be automatically marked
   done."*

   The moment a piece of work goes live, marking its item done is **part of that work, not a separate
   errand.** Put the ✅ banner on the item where it sits, add it to the DONE index at the foot with
   the date and the commit, and mention it in your report. **Never ask permission to close a finished
   item.** Closing it is not a change to the list — it is the record catching up with what is already
   true. Asking him to confirm what he can see for himself is the exact overhead this rule exists to
   remove.

   **This applies to the whole file**, not just the numbered OPEN items — the M items, the I items,
   and the standalone sections all get closed the same way when the work behind them lands.

   **The one thing that still needs care: only close what you have actually verified shipped.**
   "I think that was done" is not checking. Look at the live site, or the code, or the commit. If you
   cannot confirm it, **leave it open and say why** — recording something as finished when it isn't
   is the one failure this rule must never cause. Verify everything; ask nothing.

   ---

   **🟢 ITS COMPANION RULE — WRITING TO THIS FILE NEVER NEEDS PERMISSION.**
   *Standing rule, added 2026-09-02. In his words: "Whenever I tell you to add something to the to do
   list, I don't want to have to give you permission… I want you to add it without a single
   permission. Because when I ask you to add something, it's because I don't have time now."*

   **Adding, editing, closing, reordering, reading — none of it requires approval.** Do not ask, and
   **do not ask clarifying questions before writing either.** Write it down first in his own words,
   confirm in one line, and raise any question *after* it is captured. A question asked before the
   item is written costs him the very minute he was trying to save.

   **🔴 THE DISTINCTION THAT MUST NOT BE MISREAD.** The approval rules in
   [CLAUDE.md](CLAUDE.md) — read it back first, preview before you build, wait for his go — govern
   **code, the website, and anything that ships or is published.** Those stand, completely
   unchanged. **This file is not code and it ships nothing.** Notes and to-do files are exempt.
   Nothing written here reaches a client or changes a page.

   **Why:** the whole value of this list is that he can offload something in three seconds while he
   is in the middle of something else. A permission prompt turns a three-second thought into a
   conversation, and the thing he was trying not to lose gets lost. **If you find yourself asking
   whether you may write to this file, the answer is yes.**

4. **Never remove or reword an item on your own initiative.** If an item looks wrong, stale or
   already handled, say so and let Shimon decide. **Closing a finished item under rule 3 is not
   covered by this** — that one is required, not optional. This rule governs changing what an item
   *says*; rule 3 governs recording that it is *done*. They do not conflict.

**How Shimon uses it.** Just edit it. It is a plain text file — add a line, cross something off, no
special format to get right. If the formatting ends up untidy, Claude tidies it, it never argues
about it.

---

## 📐 HOW EVERY ITEM IS BUILT — read this before answering a question about one

**Added 2026-08-27, at Shimon's instruction.** In his words: *"make sure you know context of every
item cause sometimes ill ask you for more context on a specific to do item so make sure you
understand all of them."*

Every item on this list has **two layers**:

1. **The item itself** — plain English, describing what Shimon would see on the page and what it
   costs him. This is the part written for him. No file names, no jargon.
2. **A block underneath marked 📎 CONTEXT FOR CLAUDE** — the findings behind it: what was actually
   checked, where, the measurements and evidence, and what would have to change to close it. This
   part is technical on purpose.

**The rules that make this work:**

- **When Shimon asks for more context on an item, READ ITS 📎 BLOCK AND ANSWER FROM THAT.** Do not
  re-derive it, do not re-audit the site, and do not guess. The block exists precisely because the
  Claude that found these things is gone. Then translate it into plain English for him — the block
  is your source, not your script.
- **The 📎 blocks are never read out to Shimon as-is.** They are reference material. He asked for
  plain English and jargon-free answers; that hasn't changed.
- **When you learn something new about an item — write it back into its block**, dated. If you check
  a finding and it has changed, say so in the block rather than silently correcting it. The block is
  meant to accumulate.
- **Every block records its provenance** — which audit found it and when — so a future Claude knows
  how old the evidence is. Anything measured on a live site is a measurement taken on a date, not a
  permanent fact. Re-check before relying on it.

**A note on the order.** On 2026-08-26 Shimon approved adding the findings of a design audit of the
whole site to this list. The items are in the order that audit recommended acting on them — most
costly first — so the numbers changed on that date. Nothing was dropped. Where the audit found more
about something already on the list, it was folded into that item rather than added as a second one.

---

## OPEN

### ★ FIRST ON EVERY LIST — What the free plans themselves can do to the firm

**Added:** 2026-10-09 · **A pointer. The full entry, and the only copy to update, is at the top of
the practice manager's list:** `accounting-practice-manager/docs/TODO.md`, "★ FIRST ON EVERY LIST".
Read that one before answering any question about it.

In one breath: the hosting company's free plan forbids business use, and all four sites are on it,
this website included. The portal's database has no backups. The returns are safe because Shimon
keeps his own copies, but the record of who viewed and downloaded what would be lost for good. The
pause that took the portal down on 9 October is now kept off by a nightly check, which reduces the
risk but doesn't guarantee against it. Removing all of it costs about $50 a month. Some facts can
only be seen in his own dashboards, including the hirsch.cpa domain's renewal date, and the master
entry lists them.

### 1. Anyone who types hirsch.cpa gets a browser security warning

**Added:** 2026-08-26 · **Updated 2026-08-26** — Shimon asked for this directly, and the design
audit the same day found the situation is worse than the domain simply not being connected

In his words: **"We have to connect the real domain of hirsch.cpa."**

Here is what a visitor actually sees today if they type **hirsch.cpa** into a browser:

- A **full-screen red security warning** — *"Your connection is not private."*
- If they click past the warning, they land on a **blank generic hosting page**. Not the firm's site.
- **www.hirsch.cpa** does exactly the same thing.

So the domain is not sitting unused. It is pointed at a parking server that actively serves a warning
screen to anyone who visits.

Moving the site is two jobs, not one. Point the domain at the real site, and correct the "official
address of this page" tag — the one search engines follow — which is currently set to the temporary
address on every one of the twelve pages.

**Why it matters:** hirsch.cpa is the domain in the firm's email address. It is on the signature, on
cards, on letterhead. Anyone who does the obvious thing — reads an address ending in @hirsch.cpa and
types the part after the @ into a browser — gets a warning screen of exactly the kind people are
taught to associate with fraud. For a firm that handles other people's financial information, that is
the most damaging thing on this list, and it happens before a prospective client has read a single
word the firm wrote. It also means the site that works is the one nobody can find, and the one people
do find is broken. And if the site is moved without correcting those tags, search engines keep being
pointed at the old address until every page is fixed.

**Related:** the client portal is on a temporary address too, and this site sends clients there, so
the two are worth doing as one piece of work.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26. Shimon's own request for the domain predates the audit, same date.*
>
> **What was found.** `hirsch.cpa` and `www.hirsch.cpa` both resolve to `44.198.11.225`, a shared
> registrar parking/forwarding host. Nameservers are `standard3.encirca.net` / `standard4.encirca.net`
> (EnCirca, the registrar). The domain is live — it is not unregistered and not unresolving.
>
> **Over HTTP:** returns 200 with a cPanel default placeholder — the body is a meta-refresh to
> `/cgi-sys/defaultwebpage.cgi`. Both apex and www.
>
> **Over HTTPS:** the host presents a Let's Encrypt certificate with `CN=nil.cpa`, issuer
> `CN=YR1, O=Let's Encrypt, C=US`, valid 2026-07-11 → 2026-10-09. Its SAN list carries roughly 100
> unrelated domains (`1041.cpa`, `aa.cpa`, `nil.cpa`, `forwarding.encircalabs.com`, and so on).
> **`hirsch.cpa` is not among them.** A browser therefore fails the name check and shows the
> interstitial (`ERR_CERT_COMMON_NAME_INVALID`). This is why the audit's browser tool refused to
> navigate to it.
>
> **Mail is unaffected and must stay that way.** MX → `hirsch-cpa.mail.protection.outlook.com`
> (Microsoft 365). Any DNS change must leave the MX and any SPF/DKIM/DMARC records alone — breaking
> firm email while fixing the website would be far worse than the problem being fixed.
>
> **The real site** is at `hirsch-cpa-website.vercel.app`, served by Vercel, HSTS present
> (`max-age=63072000; includeSubDomains; preload`), all 12 pages returning 200.
>
> **The hard-coded address tags.** Every page carries `<link rel="canonical">` plus `og:url`,
> `og:image` and `twitter:image` all absolute to `https://hirsch-cpa-website.vercel.app/...`. That is
> 12 canonicals plus roughly 3 more absolute URLs per page. Also: `/robots.txt` and `/sitemap.xml`
> both 404 — neither file exists in the repo.
>
> **What would close it.** (a) Add `hirsch.cpa` + `www` as domains in the Vercel project and point
> DNS at Vercel, letting it issue a valid certificate; (b) remove or bypass the EnCirca parking host;
> (c) update canonical / `og:url` / `og:image` / `twitter:image` on all 12 pages to the new host;
> (d) add `robots.txt` and `sitemap.xml`. Steps (a) and (c) must land together or search engines keep
> being pointed at the vercel.app host.
>
> **Note on HSTS.** The vercel.app response includes `includeSubDomains; preload`. Worth checking the
> preload implications before the cutover rather than during it.

---

### 2. The contact form does not work at all — it must send an email to the firm

**Added:** 2026-08-26 · **Updated 2026-08-26** with what Shimon wants it to do, and again with what
the design audit established by testing the live form

Someone visits the Contact page, fills in their name, email, phone and message, clicks **Send
message** — and nothing happens. No email arrives at the firm. No confirmation goes back to them. Not
even an error message. The button is not connected to anything.

**What Shimon wants**, in his words: **"We have to connect the form that when you press send, it
sends an email to the company's email."**

So the intended behaviour is settled: pressing Send delivers the message to the firm by email.

**What the audit saw when it filled the form in and pressed Send on the live site.** Nothing changed
on the screen at all — no confirmation, no error, not even the button looking pressed. The details
the visitor typed just sit there in the boxes. Nothing left the browser. There is more than one
reason it can't work, so this is not one small wire to reconnect.

**Fix this at the same time — the same four boxes are unusable with a screen reader.** The labels
above them (Name, Email, Phone, How can we help?) are visible on screen but are not connected to the
boxes underneath in a way that reading software can follow. A blind visitor hears "edit text, blank"
four times with no idea what goes where. The state chooser on the Track Your Refund page has the same
problem. There is no point wiring up a form that a portion of visitors cannot fill in, and connecting
the labels is the smallest job on this whole list.

**Still to be decided — ask him, don't assume:**

- **Which address** the messages should go to. He said "the company's email" without naming it.
- Whether the person who filled the form should get a confirmation back, and what it should say.

**Why it matters:** this is the item with the clearest business cost. Every prospective client who
used the form instead of phoning or emailing believes they got in touch with the firm, and the firm
never heard from them. There is no way to find out how many people that has been. It is made worse by
item 4: **Book a call** is the most repeated button on the site — seven times on the home page alone —
and every one of them leads to this same page.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26, verified against the live site. Shimon's instruction on intended behaviour predates the
> audit, same date.*
>
> **Where.** `contact.html`, the `<form class="cform reveal">` block.
>
> **Three independent reasons it cannot work** — all three must be fixed, fixing one changes nothing:
>
> 1. The button is `<button type="button" class="btn gold lg">Send message</button>`. `type="button"`
>    does not submit by specification, it carries no `onclick`, and no script anywhere on the page
>    binds a handler to it. The only inline script on the page is the mobile menu plus the
>    IntersectionObserver reveal.
> 2. The `<form>` has no `action`, no `method`, no `id` and no `onsubmit`. Even a real submit event
>    would have nowhere to go.
> 3. None of the four controls has a `name` attribute. Even a working submit would post four empty
>    values.
>
> **Live evidence (2026-08-26).** The audit instrumented `fetch`, `XMLHttpRequest.open`,
> `navigator.sendBeacon`, the form's `submit` event and `beforeunload`, filled all four fields, then
> clicked the button. Result: **0 network calls, 0 submit events, no navigation, no DOM mutation, URL
> unchanged, fields still populated.** The browser's own network log for the page showed only
> `contact.html`, `site.css` and `logo-emblem.png`. Nothing was transmitted anywhere, so this test
> left no trace and sent no message to the firm.
>
> **Accessibility, same form.** Four `<label>` elements, none with a `for` attribute; the four
> controls have no `id`, so nothing is programmatically associated — all four report
> `labelled: false`. The visible text is carried only by placeholders, which screen readers treat as
> a hint, not a name. Same defect on `track-refund.html`: `<select class="state">` has no `<label>`
> and no `aria-label`.
>
> **Constraint that shapes the fix.** This is a static site on Vercel with no backend and no build
> step — there is no server to post to. Delivering email needs either a third-party form endpoint or
> a Vercel serverless function plus a mail provider. The firm already uses Microsoft 365 for mail and
> Brevo appears elsewhere in the practice's stack; **do not pick one without asking Shimon** — the
> destination address is already flagged as his decision.
>
> **What would close it.** Give each control a `name` and an `id`; point each `<label for>` at its
> control; add `required` where appropriate; make the button `type="submit"`; add a real submission
> path with visible success and failure feedback; and add spam protection (honeypot or similar) since
> a working public form will attract it. Then item 3's first bullet stops being untrue.

---

### 3. The privacy policy describes things the site does not actually do

**✅ DONE — REWRITTEN AND LIVE 2026-09-15, commit `68b9eda`. He approved it by name. The standing rule below never closes.**

**What was untrue and is now gone.** The policy said information is collected when you fill out the contact form: the form sends nothing, so nothing was collected. It said the site may use cookies and analytics: it uses neither. It offered an unsubscribe link for marketing email the firm does not send from this site. It named scheduling providers that are not connected.

**What it now says, all of it checked against the site itself:** the site asks you for nothing, sets no cookies, runs no analytics and stores nothing on your device; the hosting provider keeps ordinary server records; **the calculators run entirely in your browser and the figures you type are never sent to us or saved**; and the client portal is a separate site with its own sign in.

> **🔁 STANDING RULE, ADDED 2026-09-15 AT HIS INSTRUCTION. THIS ITEM NEVER CLOSES FOR GOOD.**
> **Whenever the site changes, check whether this policy is still true**, and fix it in the same pass. It is not a page that gets written once. It went stale before because the site changed underneath it, and that is the normal way this goes wrong, not an unusual one.
>
> **The three changes that will make it untrue next, in order of likelihood:**
> 1. **Fixing the contact form (item 2).** The moment it actually sends, the policy must say again that information is collected through it, what is collected, and where it goes. **Item 2 is not finished until this page is updated in the same change.**
> 2. **Adding analytics of any kind.** The policy now states plainly that there are none, and there is no cookie banner because there is nothing to consent to. Add a tracker and both statements become false on the same day.
> 3. **A calculator that sends anything anywhere.** All of them are client side today and the policy says so. Anything that posts figures to a server breaks that promise.
>
> **Checked on 2026-09-15 against the site as it then stood:** three calculators live, no cookies, no analytics, no working form, no external scripts beyond the font files.

**Added:** 2026-08-26 · **Updated 2026-08-26** — the audit checked the whole policy against the live
site and found four statements, not one

The privacy policy tells visitors that the firm collects their details through the contact form. It
doesn't, because the form doesn't work. Checking the rest of the policy against what the site
actually does turned up three more:

- It says information is collected when someone **books a call**. There is no booking system — see
  item 4.
- It says the site may automatically collect browser type, device and pages visited **through
  cookies**. The site sets no cookies and has no visitor tracking of any kind. This one was confirmed
  on the live site.
- It says visitors can **opt out of marketing emails by following the unsubscribe link**. There are
  no marketing emails.

One more thing to decide on rather than fix: the site loads its lettering from Google, so every
visitor's internet address is passed to Google each time a page opens. It is the only outside company
the site talks to, and the policy does not mention it.

**Why it matters:** it isn't a data-protection problem — information that was never received cannot
be misused. But the policy currently says several things that are untrue, and those are published
statements a regulated practice is accountable for. **Two** of the four — the contact form and the
booking — stop being untrue the moment items 2 and 4 are fixed, which is why those belong together.
The other two do not fix themselves: the cookie sentence stays untrue unless visitor tracking is
actually added, and the unsubscribe sentence stays untrue unless the firm actually starts sending
marketing emails. Both of those need the policy edited regardless of what else happens.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26. The contact-form line was already known before the audit; the other three are new.*
>
> **Where.** `privacy.html`. Policy is dated "Last updated: August 2026".
>
> **The four statements, with the section each sits in:**
>
> | Section | The claim | Reality on 2026-08-26 |
> |---|---|---|
> | Information we collect | "when you fill out our contact form" | Form transmits nothing — item 2 |
> | Information we collect | "book a call" | No booking system exists — item 4 |
> | Information we collect | "may also automatically collect … browser type, device, and pages visited, through cookies and similar technologies" | **Confirmed false on the live site:** `document.cookie` is empty, there are zero `<script src>` tags on any page, and no analytics tag appears anywhere in the source |
> | Your choices | "opt out of any marketing emails by following the unsubscribe link" | No marketing email system, no unsubscribe link |
>
> The cookie sentence is hedged with "may," so it is arguably defensible; the contact-form sentence is
> not hedged at all. Shimon should decide whether hedged-but-inaccurate is acceptable to him.
>
> **Undisclosed third party.** Every page preconnects to `fonts.googleapis.com` and
> `fonts.gstatic.com` and loads a stylesheet from Google (Fraunces + Inter). That passes the
> visitor's IP to Google on every page view. "How we share information" lists "hosting, email, and
> scheduling providers" and does not cover it. Two ways out: name it, or self-host the fonts and
> remove the third party entirely — self-hosting would also remove the only cross-origin request the
> site makes.
>
> **One more claim, tracked separately.** "Client confidentiality" says documents in the client
> portal "are protected by access controls and encryption." That is a statement about the portal, not
> this site, and it sits next to Question C — don't treat it as verified here.
>
> **What would close it.** Edit the four statements to match reality, in the same change as items 2
> and 4 where they overlap, and bump the "Last updated" date. Rule 7 in `CLAUDE.md` governs this:
> a published statement that has become untrue is part of whatever change made it untrue.

---

### 4. The "book a call" buttons must let a visitor book a slot straight away

**Added:** 2026-08-26

In his words: **"We have to connect the book a call buttons to a calendar that they should be able to
book right away."**

The book-a-call buttons on the site don't lead to a real booking today. Shimon wants a visitor to
click one and book a time there and then — not send a request and wait to hear back.

**What the audit added.** The button is the single most repeated thing on the site: seven times on
the home page, three to five times on every other page, twelve pages in total. Every one of them
leads to the Contact page — the page whose form does nothing (item 2). So the site's main invitation
to get in touch currently promises a calendar, delivers a message form instead, and that form
silently discards the message.

**Still to be decided — ask him, don't assume:**

- **Which calendar or scheduling service** he wants used. He hasn't named one, and this is the
  decision everything else waits on.
- Whose calendar the bookings land in, how long a slot should be, and when he is available.
- What the visitor sees after booking, and whether he wants to be notified.

**🔗 Answer this together with the portal.** Shimon has separately asked for a book-a-call button in
the client portal (**item 10** on the portal's list). The two almost certainly want the **same**
scheduling destination, so the moment he says which calendar to use, both items are answerable at
once. Don't decide one without the other.

**Why it matters:** a prospective client who wants to speak to the firm is as close to becoming a
client as a website visitor gets. A button that doesn't lead anywhere loses them at exactly that
point — the same failure as the contact form in item 2, on the other likely route in.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon's own request,
> 2026-08-26; counts and link-tracing added by the design audit (Audit B), 2026-08-26.*
>
> **Exact counts of the phrase "Book a call" per page** (measured 2026-08-26):
> `index.html` 7 · `contact.html` 3 · `privacy.html` 3 · `terms.html` 3 · `tax-due-dates.html` 3 ·
> `track-refund.html` 3 · each of the six pages in `services/` 5 each. Every instance is an `<a>`
> pointing at `contact.html` (or `../contact.html` from the services folder). Three of the counts on
> each inner page come from the header button, the mobile menu button and the footer link, so the
> visible-on-screen count is lower than the raw count — say "on every page" rather than quoting the
> raw number to Shimon.
>
> **There is no scheduling integration of any kind** anywhere in the source — no embed, no script, no
> outbound link to any booking service.
>
> **Live working example on file.** Item R1 in the References section is another CPA firm's site that
> does exactly this: an inline Calendly embed for a 30-minute discovery call. Recorded as an example
> of the mechanism, **not** as a recommendation — Shimon has not said which service he wants, and
> that decision is explicitly his.
>
> **What would close it.** Once he names a service: either embed it on a new booking page and repoint
> every "Book a call" link at it, or repoint them at the provider's hosted page. Whichever is chosen,
> the same destination should serve the portal's item 10. Then item 3's second bullet stops being
> untrue. If the buttons go to a real calendar, consider whether the Contact page's form is still the
> right destination for anything, or whether its wording needs to change.

---

### 5. The whole site disappears if a visitor's browser blocks scripts

**✅ DONE 2026-08-27 — shipped in commit `4fd195e`.** Content is visible by default now; the animation is layered on top. Same fix as M1.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

**Added:** 2026-08-26 · *found in the design audit*

Every block of text on the site fades in as you scroll down. Until that fade happens the text is
invisible. If the small piece of behind-the-scenes code that triggers it doesn't run, nothing ever
becomes visible. Tested on the live site: the home page came up as a **blank cream screen** with only
the header bar and the footer showing — the main headline included. Ten of the twelve pages behave
this way. Privacy and Terms don't, because those two were already made static.

On a phone it is worse: the menu button also depends on that same code, so the same visitor gets a
blank page **and** no way to navigate off it.

**Why it matters:** this is uncommon but not exotic — locked-down company IT departments are the
usual cause, which is exactly the kind of business client the firm wants. The risk is out of all
proportion to the cause: these are plain, ordinary pages that do not need any of that code to be
readable. A decorative touch is currently sitting on top of a single point of failure for everything
on the page.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26.*
>
> **🔗 SAME FIX AS M1 IN THE MOTION SECTION — BUILT ONCE, ON 2026-08-27, under this item.** M1 is
> satisfied by it; **do not build it a second time.** See M1's block for the implementation detail.
> Built but **not yet deployed** — it is waiting alongside items 7, 9 and 12.
>
> **Mechanism.** `assets/site.css` set `.reveal{opacity:0;transform:translateY(18px);transition:…}`
> and `.reveal.in{opacity:1;transform:none}`. The inline script at the bottom of each page uses an
> `IntersectionObserver` to add `.in` when an element scrolls into view. No script, no `.in`, so
> `opacity:0` is permanent.
>
> **Evidence (2026-08-26).** The home page was loaded in an iframe with `sandbox="allow-same-origin"`
> and no `allow-scripts`, i.e. scripting disabled. Result: **22 of 22 `.reveal` elements at computed
> opacity below 0.1, the `<h1>` at exactly `0`.** `body.innerText` still measured 2855 characters —
> the content is present in the DOM and readable by machines, it is simply painted invisible. So this
> does **not** hurt SEO, and Google renders JS anyway; the harm is to human visitors only.
>
> **Per-page `.reveal` counts:** `index.html` 22 · `contact.html` 3 · `tax-due-dates.html` 4 ·
> `track-refund.html` 4 · each `services/*.html` 3 · `privacy.html` 0 · `terms.html` 0.
>
> **Privacy and Terms are already exempt** — commit `93c2878` ("Privacy + Terms: static (no scroll
> animation)") removed it from those two deliberately. That is a precedent worth citing to Shimon: he
> has already decided the animation was wrong somewhere.
>
> **Mobile compounding.** At ≤900px `.nl{display:none}` hides the desktop nav and the burger's only
> handler is `onclick="toggleMenu()"`. No script means no navigation at all on a phone.
>
> **The fallback pattern is already in the file.** `@media(prefers-reduced-motion:reduce)` already
> resets `.reveal` to `opacity:1;transform:none;transition:none`. The same override under a
> `<noscript>` block — or inverting the default so `.reveal` is visible until a script adds an
> "animate" class — would close this without touching the animation for everyone else.
>
> **What would close it.** Invert the default (visible unless JS opts in), or add a `<noscript>`
> stylesheet override, on the ten affected pages. Under Rule 2 in `CLAUDE.md` this changes how the
> site looks in an edge case, so show him a preview before building.

---

### 6. The lines saying the firm is licensed are the hardest text on the page to read

**✅ CLOSED 2026-09-15 — his decision, not work.** In his words: *“it’s good this way, leave it.”* The measurements in the block below still stand; he has read them and chosen to keep the type as it is. **Do not raise this again, and do not “fix” the contrast in passing.**

**Added:** 2026-08-26 · *found in the design audit*

The palest grey text on the site is used for exactly the sentences doing the most work to establish
credibility: *"Licensed CPAs · Members of the AICPA & NYSSCPA"* on the home page, and *"Licensed
Certified Public Accountants based in New York"* lower down. Both sit below the accepted standard for
readable text. The line directly under the logo reading *"Certified Public Accountants"* is set in
tinier type than the small print in the footer.

The gold **Book a call** button — white lettering on gold — also lands just under the standard, as do
the round **CPA** badge and the small gold "CPA" beside the logo.

**Why it matters:** nobody will call any of this broken, and it does not stop anything working. But
the sentences telling a prospective client that this is a licensed professional practice are the ones
a middle-aged reader has to squint at, and the main button on the site is slightly harder to read than
it should be. A darker shade of the same grey and the darker gold already used elsewhere on the site
would settle all of it without changing the design.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26. Ratios computed with the standard WCAG 2.x relative-luminance formula against the live
> rendered DOM, not estimated by eye.*
>
> **Failures — WCAG AA needs 4.5:1 for normal text, 3:1 for large (≥24px, or ≥18.66px bold):**
>
> | Element | Colours | Size / weight | Ratio | Needs |
> |---|---|---|---|---|
> | `.microtrust` "Licensed CPAs · Members of the AICPA & NYSSCPA" | `#8B7E6C` on `#FBF8F2` | 13.5px / 400 | **3.74** | 4.5 |
> | `.about .creds` "Licensed Certified Public Accountants based in New York …" | `#8B7E6C` on `#F6F0E5` | 14px / 400 | **3.49** | 4.5 |
> | `.bt .subttl` "Certified Public Accountants" under the logo | `#8B7E6C` on `#FBF8F2` | **9px** / 400 | **3.74** | 4.5 |
> | `.btn.gold` "Book a call" | `#fff` on `#9C7430` | 15–16px / 600–700 | **4.24** | 4.5 |
> | `.cpabadge` round CPA seal | `#fff` on `#9C7430` | 18px / 600 | **4.24** | 4.5 |
> | `.bt .nmrow .c` small gold "CPA" by the logo | `#9C7430` on `#FBF8F2` | 16px / 800 | **4.00** | 4.5 |
> | `.foot .sb` and `.copy` footer small print | `#8B8271` on `#231F1A` | 12–12.5px / 400 | **4.31** | 4.5 |
>
> The 9px `subttl` is the worst of it — 9px is below any sensible floor regardless of contrast.
>
> **Already passing, do not "fix":** `--gold-d #7C5A22` on white **6.28**, on cream **5.54**; footer
> body `#B8AC98` on `#231F1A` **7.33**; `.info .k` `#CBA968` over the dark overlay ~**7.8**.
>
> **Known false positives — do not re-flag these.** An automated sweep also reported "Let's talk",
> its sub-line and the Phone/Email/Office labels as failures. They are **not**. Those sit in `.cband`,
> which has a skyline photo plus an 80–86% dark overlay; the script walked up to the page background
> instead of the overlay. They are white-on-near-black and comfortably pass.
>
> **The cheap fix.** `--gold-d` (`#7C5A22`) already passes everywhere it is used. Swapping the button
> background from `--gold` to `--gold-d`, darkening `--muted` (`#8B7E6C`) a step, and raising the 9px
> line would clear the whole table without altering the design language. All are single values in
> `:root` in `assets/site.css` — but `--muted` and `--gold` are used site-wide, so changing them
> touches every page. Rule 2: preview before building; Rule 3: this is one change, not a restyle.

---

### 7. One state's refund link is dead, and about a dozen don't land where the page promises

**✅ DONE 2026-08-27 — shipped in commit `4fd195e`.** Maine fixed; 11 others now go straight to the tracker. Oklahoma deliberately unchanged.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

**Added:** 2026-08-26 · *found in the design audit*

Every link on the site was checked. The Track Your Refund page offers forty-two state links — the
other nine states have no income tax and are correctly shown as notes rather than links — plus the
federal one. Forty-one of the forty-two work. The exception is **Maine**: choosing it takes the
visitor to a bare error page reading *"Forbidden — You don't have permission to access this
resource."* Maine's tax department is working fine; the address on the site is simply out of date.

Separately, the page tells visitors it will take them "straight to its official refund tracker," and
for about a dozen states — Arkansas, Delaware, Hawaii, Illinois, Indiana, Louisiana, Mississippi,
Montana, Nebraska, Oklahoma, Pennsylvania and Washington DC — it drops them on the state tax
department's front page instead, leaving them to find the refund page themselves.

The federal link is exact — it lands directly on the IRS refund form.

**Why it matters:** a client who followed the firm's own link to a dead error page will assume the
firm's site is broken, not Maine's. The dozen imprecise links are a smaller thing, but the page makes
a promise it doesn't quite keep.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26. **All external links are a snapshot — state URLs rot. Re-check before quoting these.***
>
> **Where.** `track-refund.html`, the `<select class="state" onchange="goState(this)">`. `goState`
> does `window.open(value,'_blank','noopener')` then resets the index.
>
> **Arithmetic, so the numbers are quotable.** 51 `<option>` entries = 50 states + Washington DC.
> Nine are `disabled` with a "— no state income tax" note (AK, FL, NV, NH, SD, TN, TX, WA, WY).
> **42 live links.** 41 respond, 1 does not. An earlier draft of the audit said "51 links, 50
> working" — that was wrong and was corrected on 2026-08-26; do not reintroduce it.
>
> **The broken one.** Maine → `https://portal.maine.gov/refundstatus/refund` returns **403
> Forbidden** both to a scripted request and in a real browser (page title "403 Forbidden", body
> "You don't have permission to access this resource"). Not a bot-block — genuinely dead.
> `https://www.maine.gov/revenue/` is alive and carries a working "Check Individual Income Tax Refund
> Status" card; the replacement URL should be taken from there at fix time.
>
> **Three links 403 to scripted checks but work in a real browser — do not flag these as broken:**
> the IRS (`https://sa.www4.irs.gov/wmr/`, verified loading the real refund form asking for SSN/ITIN,
> tax year, filing status and exact amount), Massachusetts, and — separately from its genuine failure
> — Maine's host. Always confirm a 403 in a browser before calling a link dead.
>
> **The twelve that land on a portal front page rather than a refund page:** Arkansas (`atap`),
> Delaware, Hawaii (`hitax`), Illinois (`mytax`), Indiana (`intime`), Louisiana (`latap`),
> Mississippi (`tap.dor`), Montana (`tap.dor`), Nebraska, Oklahoma (`oktap`), Pennsylvania
> (`mypath`), Washington DC (`mytax`). Several of these states genuinely have no deep-linkable refund
> page — the tracker sits behind a login — so this may be unfixable for some, and the honest fix
> could be softening the page's wording instead of chasing URLs.
>
> **NH note:** listed as "no state income tax", correct as of 2026 — its interest-and-dividends tax
> was repealed effective 2025. Do not "correct" this back.
>
> **Also here:** the `<select>` has no `<label>` and no `aria-label` — that half of the fix belongs
> with item 2, where the form-labelling work is.

---

### 8. The firm's address has no ZIP code anywhere on the site

**✅ CLOSED 2026-09-15 — his decision, not work.** In his words: *“don’t need one, drop it.”* **Do not add a ZIP code to the address, and do not raise it again.** Note this also settles the address half of idea I25.

**Added:** 2026-08-26 · *found in the design audit*

The address appears four times as **65 S 11th Street, Brooklyn NY** — written two slightly different
ways on different pages — with no ZIP code and no suite number.

**Why it matters:** clients post tax documents to the firm. And an incomplete address holds a firm
back in local search results — when someone searches for an accountant near them, a complete and
consistently written address is one of the things that decides whether the firm appears at all.

The phone number and email address, by contrast, are correct and identical on all twelve pages, and
tapping them on a phone dials or opens mail properly.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26.*
>
> **The four instances and their two forms:**
> - `65 S 11th Street, Brooklyn NY` (no comma before NY) — `index.html` contact band, `contact.html`
>   info panel.
> - `65 S 11th Street, Brooklyn, NY.` (comma, trailing full stop) — `privacy.html` and `terms.html`,
>   both in their "Contact us" paragraph.
>
> No ZIP, no suite/floor, on any of them. **Claude does not know the correct ZIP or whether there is
> a suite number — ask Shimon, never guess an address for a regulated firm.**
>
> **Consistent and correct, for contrast:** `(347) 486-2780` appears 16 times, always with
> `tel:+13474862780`; `info@hirsch.cpa` appears 30 times, always with a `mailto:`. Both verified
> identical across all 12 pages. (Whether the mailbox is actually read is Question A.)
>
> **The local-search angle.** Consistent name/address/phone across the web is what ties a site to a
> Google Business Profile. Two spellings and a missing ZIP weakens that. There is also no
> `LocalBusiness`/`AccountingService` structured-data markup anywhere on the site — worth raising
> with Shimon as a separate decision if he cares about local search, **not** something to add
> unasked (Rule 3).

---

### 9. A mistyped or out-of-date link shows a blank white page

**✅ DONE 2026-08-27 — shipped in commit `4fd195e`.** New page-not-found page, served for wrong addresses at any depth.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

**Added:** 2026-08-26 · *found in the design audit*

Get a page address slightly wrong, or follow an old link that no longer exists, and the visitor gets a
**completely blank page** — no logo, no menu, no message, no way back to the site.

**Why it matters:** small, but it is the one moment when someone is already lost, and the site hands
them a dead end instead of a door back in.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26.*
>
> **Evidence.** `https://hirsch-cpa-website.vercel.app/<any-missing-path>` returns HTTP 404 with
> `Content-Type: text/plain; charset=utf-8` and a 79-byte body that reads as empty in a browser. This
> is Vercel's default handler — there is no `404.html` in the repo and no `vercel.json` routing
> config.
>
> **Worth knowing:** no internal link on the site is broken. All twelve pages and all fifteen assets
> return 200; every `href` in the source resolves to a real file. This 404 page is only reached by a
> mistyped URL or a stale external link — so it is genuinely low-frequency, and should be described
> to Shimon that way rather than as "the site has broken pages."
>
> **What would close it.** Add a `404.html` carrying the site's own header, footer and a line back to
> the home page. On Vercel a root-level `404.html` is picked up automatically for static projects.
> Rule 2 applies — it is a new page with a look, so preview it first.

---

### 10. The six service pages look different from the rest when shared

**Added:** 2026-08-26 · *found in the design audit*

When a page is shared on LinkedIn, WhatsApp or in a message, a little preview card appears. A recent
tidy-up of those cards reached the six main pages but missed the six service pages. So sharing
Contact shows a card reading *"Contact • Hirsch CPA"*, while sharing Tax Preparation shows *"Tax
Preparation — Hirsch CPA"* with a long dash instead.

**Why it matters:** only visible when someone shares a link — which is precisely the moment the firm
is being passed on to someone new.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26.*
>
> **The cause.** Commit `08177cb` ("Clean up social preview titles: drop em-dashes, fix homepage
> og:title") replaced em-dashes with `•` in the social tags — but only on the six root-level pages.
> The six files in `services/` were not touched.
>
> **Current state, measured 2026-08-26:**
> - Root pages — `og:title` / `twitter:title` use `•`: e.g. `Contact • Hirsch CPA`,
>   `Privacy Policy • Hirsch CPA`.
> - Service pages — still use `—`: `Advisory — Hirsch CPA`, `Audit — Hirsch CPA`,
>   `Bookkeeping — Hirsch CPA`, `Payroll — Hirsch CPA`, `Sales Tax — Hirsch CPA`,
>   `Tax Preparation — Hirsch CPA`.
> - `og:image:alt` is split the same way: `… LLC • Certified Public Accountants` on root pages,
>   `… LLC — Certified Public Accountants` on service pages.
>
> **Not affected — leave alone:** all twelve `<title>` tags already use `·` consistently. Only the
> social/OG tags diverge.
>
> **What would close it.** Replace `—` with `•` in `og:title`, `twitter:title` and `og:image:alt`
> across the six `services/*.html` files — 18 strings. Purely mechanical, no visual change to the
> pages themselves, so Rule 2's preview requirement does not really bite here.

---

### 11. Footer links are small targets on a phone

**Added:** 2026-08-26 · *found in the design audit*

Every link in the footer is noticeably shorter than the recommended minimum for a comfortable tap, and
**Privacy** and **Terms** at the very bottom are smaller still — easy to miss and easy to hit the
wrong one.

The main phone menu is fine — properly sized, opens and closes cleanly, and the expanding sections
work correctly.

**Why it matters:** minor irritation rather than a real obstacle, but most visitors are on a phone.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26, measured on the live site at a 375×812 viewport.*
>
> **Measured tap targets below the 44×44px guideline:** all 14 footer links render **149×33px**
> (`.fcol a{padding:5px 0}` at 14px); the bottom-bar links are **Privacy 44×15px** and
> **Terms 37×15px** (`.copy` at 12.5px, inline, separated by a `·`).
>
> **Measured and passing — do not flag:** burger **44×44**; mobile menu sub-links **~47px** tall
> (`.msub a{padding:11px 4px}` at 15px); menu section buttons `.macc` ~50px; all `.btn` elements
> ~51px.
>
> **Mobile menu behaviour, verified working:** opens at `top:78px`, height 276px, expands to 674px
> with both accordions open against a `max-height` of 734px with `overflow:auto`, backdrop appears,
> `body.style.overflow` is set to `hidden` to lock background scroll, and links close the menu on
> click. This is well built — say so if Shimon asks about the mobile menu.
>
> **What would close it.** Raise `.fcol a` vertical padding and give the `.copy` links some padding.
> Both are single-line CSS changes, but they lengthen the footer on every page — Rule 2, preview it.

---

### 12. A few wording and punctuation slips

**✅ DONE 2026-08-27 — shipped in commit `4fd195e`.** Five punctuation and hyphenation corrections.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

**Added:** 2026-08-26 · *found in the design audit*

On the Due Dates page: *"An extension gives you more time to file, not more time to pay, any tax owed
is still due by the original deadline."* — that is two sentences joined by a comma where a full stop
belongs. The same pattern appears a few more times, for example *"Call or email us directly, we're
always happy to help."*

On the Payroll page: "Year end W-2" should be "Year-end", "Payroll set up" should be "Payroll setup",
and "Clean up of prior period books" should be "Cleanup of prior-period books".

The tax content itself is correct. All seven filing and extension dates were checked against the
actual rules, including the one that is easiest to get wrong — trusts and estates on extension — and
all of them are right.

**Why it matters:** nothing here misleads anyone. But small punctuation errors on a page giving tax
guidance quietly undercut the impression of precision the rest of the site works hard to create.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26.*
>
> **Comma splices** — `tax-due-dates.html` closing note: *"An extension gives you more time to file,
> not more time to pay, any tax owed is still due by the original deadline."* · `contact.html`:
> *"Call or email us directly, we're always happy to help."* Others are stylistic fragments
> ("Quick answers and clear communication, no waiting weeks to hear back") and are defensible — do
> not sweep them all up as errors.
>
> **Hyphenation / noun-verb form** — `services/payroll.html`: "Year end W-2 and 1099 preparation"
> → "Year-end"; "Payroll set up for new employees or contractors" → "Payroll setup".
> `services/bookkeeping.html`: "Clean up of prior period books that have fallen behind" → "Cleanup of
> prior-period books". Note `services/advisory.html` already gets it right ("year-end planning",
> "ahead of year end"), so payroll is the outlier, not the standard.
>
> **Minor copy drift, homepage card vs service page hero** — Audit: "delivered with rigor and
> clarity" vs "done with rigor and clarity". Payroll: "obligations are covered" vs "your obligations
> are covered". Trivial; listed only so a future Claude doesn't think it found something new.
>
> **Verified CORRECT — do not "fix" these.** All seven dates on `tax-due-dates.html` check out
> against the real rules: Mar 15 (1120-S, 1065) · Apr 15 (1040, 1120, 1041) · May 15 (990 series) ·
> extensions Sep 15 (1120-S, 1065) · **Sep 30 (1041 — 5½ months, not 6; this is the one that is
> usually got wrong)** · Oct 15 (1040, 1120) · Nov 15 (990). Also correct: Form 706 due 9 months
> after death with a 6-month extension; the note that fiscal-year and June-30 C corps differ.
>
> **Also verified clean:** a full scan for `lorem`, `ipsum`, `TODO`, `TBD`, `FIXME`, `example.com`,
> `555-` and similar found **nothing** anywhere on the site. No placeholder text was ever left behind.
>
> **Small mismatch worth knowing:** the page's own description says "return **and payment**
> deadlines" but it lists no estimated-tax payment dates. Either the description or the content is
> slightly off. Raise it, don't decide it.

---

### 13. One large photograph that is almost entirely hidden

**✅ CLOSED 2026-09-15 — his decision, not work.** In his words: *“I like it, leave it.”* The 298KB skyline image stays exactly as it is. **Do not compress, replace or remove it.**

**Added:** 2026-08-26 · *found in the design audit*

The city skyline behind the "Let's talk" panel at the bottom of the home page is by far the largest
file on the site — and it sits under a dark shade that hides roughly eighty-five per cent of it.

**Why it matters:** the site is fast overall, comfortably under a second to load, so this is not
urgent. It is simply the one obvious piece of dead weight, and it is paid for out of visitors' mobile
data.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26.*
>
> **The file.** `assets/skyline.jpg`, **298 KB** — the largest asset on the site by a wide margin.
> Used once, as the `background-image` of the `.cband` section on `index.html` only, beneath
> `.cband .cover`, which is `linear-gradient(rgba(28,23,16,.80), rgba(28,23,16,.86))`. So 80–86% of
> it is covered.
>
> **Everything else, for scale:** `svc-sales-tax.jpg` 157 KB · `svc-audit.jpg` 145 KB ·
> `svc-advisory.jpg` 111 KB · `svc-tax-preparation.jpg` 98 KB · `hero-team.jpg` 83 KB ·
> `og-image.png` 78 KB · `svc-bookkeeping.jpg` 74 KB · `svc-payroll.jpg` 69 KB · `aicpa.png` 25 KB ·
> `site.css` 21 KB · `nysscpa.png` 17 KB · `logo-emblem.png` 14 KB.
>
> **Measured performance (live, 2026-08-26).** TTFB 14 ms, DOMContentLoaded 67 ms, load event 152 ms.
> No JavaScript libraries, no analytics, no tracking. The only cross-origin requests on the whole
> site are the two Google Fonts hosts. **This site is genuinely fast — do not let a future
> "performance" push imply otherwise.**
>
> **Two related observations, not yet items:** no image carries `loading="lazy"`, and no `<img>` has
> explicit `width`/`height`. Layout shift is mostly avoided anyway because `.photo` and `.sphoto` use
> `aspect-ratio` with absolutely-positioned images. Images are not oversized for their display sizes.
>
> **What would close it.** Re-compress or downscale `skyline.jpg`, or replace it with a flat colour
> or gradient given how little shows through. Any of those changes how the home page looks — Rule 2,
> preview first.

---

### 14. Tapping About or Services on a phone hides the section heading

**✅ DONE — LIVE 2026-09-15, commit `68b9eda`.** A jump to About or Services now lands clear of the bar that stays at the top of the screen. Measured on a phone: the section label sits 87px below the bar, where it used to be hidden behind it. One line in `assets/site.css`, so it fixes every page at once.

**Added:** 2026-08-26 · *found in the design audit*

On a phone, tapping **About** or **Services** in the menu jumps down the page but leaves the small
heading label of that section tucked partly behind the bar that stays fixed at the top of the screen.

**Why it matters:** cosmetic. The visitor arrives in the right place, just slightly too far down.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26. **Derived from CSS plus a measured header height — not visually confirmed**, because the
> audit's browser pane could not scroll or screenshot. Verify on a real phone before acting.*
>
> **The mechanism.** `header` is `position:sticky;top:0` with `.nav{height:78px}` — measured 79px
> rendered, and not overridden at any breakpoint. No element on the site sets `scroll-margin-top`;
> computed value on `#about` is `0px`. A fragment jump therefore aligns the target's top edge with
> the viewport top, i.e. underneath the 79px bar.
>
> **Why desktop is nearly fine and mobile is not.** `.blk{padding:82px 0}` on desktop — 82 > 79, so
> the bar only covers the section's own padding and the content clears it by ~3px (cramped, not
> hidden). At `max-width:900px` that drops to `.blk{padding:56px 0}` — 56 < 79, so the `.tag` eyebrow
> ("ABOUT", "WHAT WE DO") ends up behind the bar.
>
> **Affected targets:** `index.html#about`, `index.html#services`, `index.html#top` — linked from the
> header nav, the mobile menu and the footer on all twelve pages.
>
> **What would close it.** `scroll-margin-top` of about 90px on the anchor targets. One line; affects
> nothing else visually until an anchor is used.

---

### 15. The copyright year is typed in by hand on every page

**✅ DONE — LIVE 2026-09-15, commit `68b9eda`.** The year keeps itself right from now on. The correct year is still written into every page, so it reads correctly even with scripts switched off; the script only keeps it current in later years.

**Added:** 2026-08-26 · *found in the design audit*

All twelve pages show 2026, which is correct today. Because it is typed in rather than worked out
automatically, on the first of January it becomes wrong on all twelve pages at once, and stays wrong
until someone edits each one.

**Why it matters:** a stale copyright year is a small thing that regular visitors do notice, and it
reads as a site nobody is looking after.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26.*
>
> **Evidence.** `© 2026 Hirsch & Co. Accounting LLC. All rights reserved.` is hard-coded in the
> `.copy` footer block of all twelve pages. A scan for four-digit years across the whole site returned
> **only** 2026, 14 occurrences — so there is no other stale date hiding anywhere. **Correct as of
> 2026-08-26; becomes wrong on 2027-01-01.**
>
> **The tension to flag rather than resolve.** The obvious fix is a line of JavaScript writing the
> current year. But item 5 is about the site depending on JavaScript too much, and a script-written
> year renders blank when scripts don't run. The alternatives are editing twelve files each January,
> or dropping the year entirely ("© Hirsch & Co. Accounting LLC"), which is legally fine and never
> goes stale. **Shimon picks — don't decide this one.**

---

### 16. Calculator 1 — savings growth (compound interest)

**✅ DONE 2026-09-02 — shipped in commits `626d9ab` → `66d8bac`.** Live at
`compound-interest-calculator.html`, reachable from a new Financial Calculators landing page.
Maths re-verified against the live page on 2026-09-02 — see the block below.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

**Added:** 2026-08-27 · **Numbered 2026-08-27** — see the
[calculator numbering](#calculators--the-permanent-numbering) section

Shimon asked for a working compound interest calculator, modelled on the one at
moneygeek.com but built in the firm's own colours, type and layout so it looks like part of his
site. A visitor puts in a starting amount, what they add and how often, the rate they expect and how
many years, and sees the balance it grows to, a chart of the growth year by year, and a breakdown of
how much was theirs, how much they added and how much was interest.

**Built as a standalone page for him to judge** on 2026-08-27, at
`C:\Users\Admin\Documents\outputs\hirsch-compound-interest-calculator.html`. Not on the site, not
deployed.

**Still to be decided — ask him, don't assume:**

- Whether he wants it published at all, and where it would sit in the menu.
- **Whether he approves the disclaimer wording** (see the block below — the exact text is recorded
  there).

**Why it matters:** it is the first thing on the list that gives the public a number with the firm's
name on it. Useful as a reason to visit the site, but a calculator that produces a figure someone
acts on is a different kind of publishing from a page that describes a service.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon's request,
> 2026-08-27, modelled on <https://www.moneygeek.com/resources/compound-interest-calculator/>.*
>
> **🔗 This is I19 in the IDEAS section becoming a real intention.** I19 ("Add a free tool or
> calculator") stays where it is as the general idea and its reasoning; **items 16 and 17 are the
> specific things he actually asked for.** Do not treat them as three separate pieces of work, and do
> not re-pitch I19 as if nothing had happened.
>
> **What it does.** Inputs: initial amount, contribution, a Monthly/Annually toggle, rate of return,
> years. Output: headline balance, a stacked bar chart of growth by year (initial / contributions /
> interest), and a four-row breakdown. Everything recalculates as you type — there is no Calculate
> button.
>
> **The maths, and how it was checked.** Monthly compounding, contributions added at the end of each
> period — the standard convention, and the one the reference uses. Verified three ways: it
> reproduces the reference's own default result ($5,000 + $150/month at 4% for 10 years = **$29,542**)
> exactly; it agrees with the closed-form annuity formula to the dollar; and the shipped JavaScript
> was run in a browser against zero rate, zero contributions, annual contributions and junk input
> without breaking.
>
> **Built with no dependencies.** The chart is inline SVG drawn in plain JavaScript — nothing is
> fetched, so it works offline and adds no third party. The firm's real stylesheet is inlined rather
> than approximated.
>
> **⚠️ The disclaimer wording is Shimon's to approve.** Currently: *"An estimate, not advice. This
> calculator is a general illustration based only on the figures you enter. It assumes the rate stays
> the same for the whole period and does not account for tax, fees, inflation, or any change in your
> circumstances — so your actual result will be different. It is not a recommendation to make any
> particular investment. Please speak to us about your own situation before acting on it."* This sits
> alongside `terms.html`, which already disclaims the site as general information only. **Do not
> publish without his sign-off on this sentence** — Rule 7.
>
> ---
>
> **✅ RE-VERIFIED ON THE LIVE SITE, 2026-09-02.** The calculator was published on 2026-09-02 across
> commits `626d9ab`…`66d8bac` and now sits at `compound-interest-calculator.html`. The maths above was
> re-checked against the **live page**, not the standalone draft: $5,000 + $150/month at 4% for 10
> years returns **$29,542**; $10,000 with no contributions at 5% for 10 years returns **$16,470**,
> matching monthly compounding to the dollar; $1,000,000 + $5,000/month at 12% for 30 years returns
> **$53,424,462**, also correct. Empty fields, letters typed into the number boxes, and a 0% rate all
> return $0 or the plain principal rather than breaking or showing an error. No console errors on the
> page. The year-by-year table reconciles: each row's start + added + growth equals its total.
>
> **📌 THE ANNUAL MODE'S CONVENTION — recorded so nobody "corrects" it later.** With **Once a year**
> selected, the contribution is treated as going in at the **end** of each year, so **year one shows
> no growth on that year's contribution.** The table reflects this: $1,200 a year at 6% for 5 years
> shows year 1 as `$0 start · $1,200 added · $0 growth · $1,200 total`, and finishes at **$6,787**.
> The rate applied each year is the effective annual rate implied by monthly compounding (6% nominal
> → 6.1678%), which is why year 2's growth is $74 on $1,200 rather than $72.
>
> **This is deliberate, internally consistent, and NOT a defect.** It is the ordinary-annuity
> convention — the same one the monthly mode uses, and the conservative reading of the two. If a
> future audit flags "year one earns nothing" as a bug, **that finding is wrong and this block is the
> answer to it.** The only genuinely open question is whether Shimon wants the page to *state* which
> convention it uses, and that is a wording decision for him, not a correction to the maths.
>
> **⚠️ Two things above are now out of date — left unaltered on purpose, per the rule at the top of
> this file.** (a) The item body still says the calculator is "Not on the site, not deployed" and
> lists publication as undecided; it is live. (b) The disclaimer recorded above as needing sign-off
> **was not the wording that shipped** — the published page reads: *"This is an estimate, not advice.
> It assumes the same return every year, which real investments do not do, and it ignores tax, fees
> and inflation, so your actual result will be different. It is not a recommendation to invest in
> anything. Talk to us about your own situation before acting on it."* Shorter, and it says the same
> things. **Whether Shimon approved that specific wording before it went live is not recorded
> anywhere — ask him, and ask at the same time whether item 16 should move to DONE.** Neither the item
> nor its status was changed without his say-so.

---

### 17. Calculator 2 — monthly mortgage payment

**✅ DONE 2026-09-03 — shipped in commit `76d83eb`, live at `mortgage-calculator.html`** and reachable
from a second card on the Financial Calculators page.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

> **The arithmetic was verified independently before it went live, not read back off its own code.**
> Every figure was re-derived from the standard amortisation formula in a separate implementation and
> compared: monthly payment, interest over the term, total repaid, total cost including the deposit.
> Five cases matched to the dollar. The 30-row schedule matched row for row, each row's start minus
> principal equals its closing balance, each row opens where the last closed, and it ends at exactly
> zero. **Cross-checked against MoneyGeek's own calculator:** $250,000 at 7% over 30 years with 20%
> down gives $1,331 there and $1,331 here.
>
> **⚠️ A note for anyone re-checking against MoneyGeek's article rather than its calculator.** Their
> worked example says $200,000 at 6% over 30 years is $1,194. The correct figure is **$1,199** — their
> prose rounds the intermediate values. Their calculator is right; their article's hand-working is
> not. **Do not "correct" ours to match their article.**
>
> **Rounding, since Shimon is a CPA and may add the column up:** each schedule row is shown to the
> whole dollar, so summing the column by hand lands $1 to $3 away from the total across 15 to 30 rows.
> That is display rounding, not a difference in method — the breakdown totals are taken from the same
> month-by-month walk that builds the schedule, so there is only ever one source of truth.
>
> **How it was published:** assembled on calculator 1's shell, not the standalone draft. Header,
> mobile menu and footer are byte-identical to calculator 1, the shared stylesheet is linked rather
> than inlined, the base64 logo is replaced by the real asset, and the no-JS fallback comes with it.
> 94KB draft became a 40KB page. Checked live at desktop and 375px: no sideways scroll, nothing
> overflowing, no console errors.

**Added:** 2026-08-27 · **Numbered 2026-08-27** — see the
[calculator numbering](#calculators--the-permanent-numbering) section

Shimon asked for a calculator that works out a monthly mortgage payment. A visitor puts in the price,
their deposit, the term and the rate, plus property tax, insurance and any HOA fee, and sees what it
would cost per month, split into where each part of the payment goes, along with the total interest
over the life of the loan.

**Built as a standalone page for him to judge** on 2026-08-27, at
`C:\Users\Admin\Documents\outputs\hirsch-mortgage-calculator.html`. Not on the site, not deployed.

**Still to be decided — ask him, don't assume:**

- Whether he wants it published, and where.
- **Whether he approves the disclaimer wording**, and separately **whether he is comfortable with the
  mortgage insurance estimate** (see the block below).

**Why it matters:** same as item 16, and slightly sharper — people make large decisions off mortgage
figures, and a lender's real numbers will always differ from any estimate.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon's request,
> 2026-08-27. No reference site was given; the input set is the conventional one.*
>
> **🔗 Same relationship to I19 as item 16** — see that item's block.
>
> **What it does.** Inputs: home price, deposit (a dollar box and a percent box that keep each other
> in step), term (30/20/15), interest rate, annual property tax, annual insurance, monthly HOA.
> Output: headline monthly payment, a donut chart splitting the payment, a legend with each
> component's dollar figure, and life-of-loan totals. Recalculates as you type.
>
> **The maths, and how it was checked.** Standard amortisation:
> `M = P·i(1+i)^n / ((1+i)^n − 1)`. Agrees with the independent form `P·i/(1−(1+i)^−n)` to the cent.
> The shipped JavaScript was run in a browser against a 0% rate, a 100% deposit, a 15-year term, junk
> input, and the two-way deposit sync — all correct, nothing crashes. Defaults ($450,000, 20% down,
> 6.5%, 30 years) give **$2,925/month** and **$459,160** total interest.
>
> **⚠️ One judgement call he has to confirm.** Mortgage insurance is added automatically when the
> deposit is under 20%, estimated at **0.5% of the loan a year**. That is a mid-range industry figure,
> not his firm's figure, and the page says so on screen. **If he is not comfortable publishing an
> assumed rate, the alternative is to drop the PMI line entirely** and note that lenders add it below
> 20% — ask him rather than deciding.
>
> **⚠️ The disclaimer wording is his to approve.** Currently: *"An estimate, not a loan offer or
> advice. This calculator is a general illustration based only on the figures you enter. It assumes a
> fixed interest rate for the whole term and does not include closing costs, lender fees, or future
> changes to your property taxes and insurance. A lender's own figures, and what you are actually
> offered, will be different. Please speak to us about your own situation before relying on it."*
> **Do not publish without his sign-off** — Rule 7.
>
> **✅ SIGNED OFF BY SHIMON, 2026-08-27. Calculator 1 is approved as it stands.**
> `C:\\Users\\Admin\\Documents\\outputs\\calculator-1-compound-interest-APPROVED-2026-08-27.html`
>
> **In his words he likes it "for now" and wants to be able to change it later.** So this is a
> **snapshot to return to, not a frozen specification.** He can change any part of it whenever he
> wants, and when he does, take a fresh snapshot with that day's date rather than editing this one.
> **Never quote it back at him as a reason not to change something.**
>
> **What he approved**, after seven rounds of his own feedback: the result as a single large figure
> under a small gold line, with no boxes; the page calculating itself on landing from the prefilled
> figures and then staying still until Calculate is pressed; the chart and table switch as two icons
> at the top right with the section title centred; the chart fitting its box at every width with no
> sideways scrolling; the other bars fading when one is pointed at; plain quiet radio buttons for
> monthly or yearly; a question mark beside each field label explaining it in plain English;
> thousands separators everywhere including inside the fields as you type; and no dashes anywhere on
> screen.
>
> **Settled in the last few rounds and included in the sign off:** years run to 120 and the rate of
> return to 100%; very large results read in plain words ("$3.12 trillion", and "more than $1,000
> trillion" once the exact figure stops meaning anything) rather than in scientific notation or
> seventy digits; **there is no "your figures changed" notice**, he disliked it, though the Calculate
> button and its behaviour stay exactly as they were; and the chart keeps the ordinary arrow cursor
> because nothing on it is clickable.
>
> **The working copy stays at `calculator-1-compound-interest.html`. Edit that one.** The snapshot
> exists only so the approved look can be recovered if a later change goes wrong.
>
> **Signing off still does not freeze it.** His words when the design was first saved were that he
> likes it "for now" and wants to be able to change it later. A sign off records what was agreed on
> a date, it is not a reason to push back on a change he asks for afterwards.

> **➡️ CALCULATOR 2 BROUGHT IN LINE, 2026-08-27.** Once calculator 1 was signed off, the mortgage one
> was rebuilt to the same settled style so he can approve it the same way. It now has: no dashes
> anywhere on screen; thousands separators everywhere including inside the fields as you type; a
> question mark beside every field explaining it in plain English, working on hover, tap, keyboard
> and Escape; a Calculate button with the page landing already worked out and then holding still
> until the button is pressed; the result as one large figure under a small gold line with no boxes;
> plain quiet radio buttons for the term instead of the filled segmented control; and the ordinary
> arrow cursor throughout.
>
> **Two deliberate differences from calculator 1, both justified:**
> - **It keeps a short muted line under the figure** saying the headline is the loan repayment only
>   and that tax and insurance come on top. Calculator 1 has no such line, but without it the
>   headline here is misleading, which is a Rule 7 problem rather than a style one. It is quiet grey
>   text now, not the yellow box it used to be.
> - **No chart or table switch.** There is no year by year data to show, so it keeps the single bar
>   comparing what you borrow against what the interest adds.
>
> **The optional tax and insurance fields also wait for the button**, like everything else, rather
> than updating as you type. That is consistent, and the note above them says so.

> **Both calculators, if they are ever published:** they would need the site's header and footer
> wired to real relative links (the previews point at the live vercel.app addresses).
>
> **➡️ REVISION 2, 2026-08-27 — calculator 1 rebuilt on Shimon's feedback.** His six points, and what
> each became:
>
> 1. **"I dont like dashes."** Every dash was removed from the interface. Verified: zero em dashes,
>    en dashes or minus signs in the visible text. The only hyphen left is inside the phone number.
>    **Treat this as a standing preference across everything, not just this page.**
> 2. **"Only the number... not the description."** The result is now three boxes, each showing a
>    figure with a short label under it (Total balance / Principal / Growth). The explanatory sentence
>    is gone. **His points 2 and 3 pulled against each other** — stripping the descriptions risks the
>    numbers becoming unidentifiable — so the labels were kept to one or two words rather than removed
>    entirely.
> 3. **Hover shows two numbers.** Pointing at a bar shows that year's **Principal** and **Growth**,
>    using his own words. An invisible full height hit area per year makes it easy to hit; it also
>    responds to tap and to keyboard focus, and carries a text fallback for screen readers.
> 4. **Table view.** The reference's table was found behind a third view tab (chart, pie, table) and
>    its columns copied exactly: Year, Starting balance, Added this year, Added so far, Growth this
>    year, Growth so far, Total balance. **Our figures match theirs row for row** ($7,037 at year 1,
>    $9,157 at year 2, $11,364 at year 3).
> 5. **Monthly or annual contributions.** The toggle is back. It had been removed during the earlier
>    simplification pass; he wants the choice.
> 6. **Calculate button, and only on press.** Nothing calculates as he types.
>
> **⚠️ The decision inside point 6, so nobody quietly reverses it.** Before the first press the
> results area shows a short empty state rather than a pre-calculated default. That is the literal
> reading of "calculate only when hitting that button". The fields still carry sensible defaults, so
> one press gives a real answer immediately. **After a result is shown, editing a field does not
> recalculate** — it reveals a notice saying the figures changed and to press Calculate again. The
> old numbers stay on screen but are openly flagged as out of date, which is safer than either
> silently showing a stale figure or wiping the screen while he is reading it.
>
> **➡️ REVISION 3, 2026-08-27 — three further changes from a screenshot review.**
>
> 1. **The contributions frequency control is now plain radio buttons**, small and quiet: a 15px
>    circle filled gold when chosen, hollow grey when not, small normal weight text, both on one
>    line, no box and no button styling. It sits directly under the contributions amount, and the
>    bold heading that used to sit above it is gone. His reference for this was the equivalent
>    control on moneygeek.com.
> 2. **The chart and table switch moved to the top right of the chart area, as two icons only**, with
>    a thin divider between them and the active one darkened. This copies the reference, which puts a
>    row of icon tabs on the right of a header line whose left side carries the section title. Our
>    title now changes with the view: "Growth over time" for the chart, "Year by year" for the table.
> 3. **The chart no longer scrolls sideways.** It is now drawn at the true pixel width of its box
>    rather than at a fixed size, so it always fits and the bars compress as the screen narrows.
>    Verified at 375, 414, 768 and 1200 pixels: all thirty bars render, the page never scrolls
>    sideways, and the year labels thin out automatically so they never collide. **It redraws on
>    window resize, and again when switching back from the table**, because a hidden pane reports
>    zero width and would otherwise draw at the wrong size.
>
> **⚠️ Careful with the standing instruction here.** Shimon has said that for this calculator,
> **"all of these changes follow the link I gave you"** — moneygeek.com is the authority on layout
> and interaction. **His site's colours still win over the reference's.** Where the two disagree on
> anything else, go and look at the reference rather than guessing from a description.
>
> **A version mix up worth knowing about.** His screenshot for this round showed a sentence under the
> big figure reading "You'd put in X of your own money and earn Y in interest on top", and asked for
> it to be deleted. **That sentence had already been removed** in revision 2, at his own earlier
> instruction. He appears to have been looking at an older download. The figures in his screenshot
> ($72,000 principal and $380,098 growth, from nothing invested at $200 a month, 10%, 30 years) were
> reproduced exactly by the current build, which confirms the maths is identical and only the
> presentation differs. **If he ever says "leave it like this" about a screenshot, check which build
> he is holding before acting on it.**

> **➡️ REVISION 4, 2026-08-27 — two more from a screenshot review.**
>
> 1. **It now works itself out on landing**, from the prefilled defaults, so the page never shows an
>    empty result. **This refines his earlier "only calculate when hitting that button" instruction
>    rather than reversing it**, and both halves are live: it calculates once on load, then does
>    **not** recalculate while he types. Editing a field only reveals the notice saying the figures
>    changed. Pressing Calculate is still the only thing that updates the numbers. Verified in that
>    exact order: land, type new figures, confirm the figure has not moved, press, confirm it has.
> 2. **The three result boxes became one figure**, matching his screenshot: a small gold line above a
>    large serif number, no boxes and no borders. Nothing sits beside it.
>
> **Checked before removing the boxes, because the principal and growth split lived in them:** that
> split is still available in three other places, so nothing was lost. The chart legend names
> Principal and Growth, hovering any bar gives that year's two figures, and the table carries
> "Added so far" and "Growth so far" columns.
>
> Tested at 320, 375, 414, 768 and 1200 pixels, with a figure as large as $12,345,678: the number
> always fits its box and the page never scrolls sideways.

> **➡️ REVISION 5, 2026-08-27 — four more.**
>
> 1. **The chart header title is gone.** It used to read "Growth over time", switching to "Year by
>    year" for the table. He asked for the first to go; **both were removed** rather than leaving the
>    header with a title in one view and nothing in the other, and the toggle now sits alone at the
>    right. Say so if he asks, since he only named one of the two.
> 2. **The "Point at any bar" helper line under the chart is gone.**
> 3. **The four fields are named in his exact words:** Initial Amount, Contributions, Rate of return,
>    Years of growth. **His capitalisation is inconsistent between the first two and the last two and
>    that is deliberate. Do not tidy it.**
> 4. **Hovering a bar fades every other bar back to a fifth of its strength** and leaves the hovered
>    year at full. It also works on keyboard focus.
>
> **⚠️ The phone case on item 4, which is the part that could have gone wrong.** There is no hover on
> a touch screen, so a tap dims the rest and there is nothing to "move away" from to undo it. A tap
> anywhere off a bar now clears it, so nobody gets stuck looking at a faded chart. Verified: tap a
> bar (figures show, rest fades), tap elsewhere (everything back). The clearing listener is attached
> **once**, not on every redraw, and the tooltip is cleared at the start of each redraw so a stale
> one cannot survive a resize or a view switch.

> **➡️ REVISION 6, 2026-08-27 — two more.**
>
> 1. **The chart header title is back, centred**, with the toggle still pinned right. It changes with
>    the view again: "Growth over time" for the chart, "Year by year" for the table. True centring
>    needs the empty column on the left to be as wide as the toggle on the right, so **below 520px
>    the panel is too narrow and the title drops to its own line with the toggle right beneath it.**
>    Verified one row and genuinely centred at 560, 768 and 1200; stacked with no overlap at 320,
>    375, 414 and 520.
> 2. **A small question mark sits beside each field label** and explains the field in plain English.
>    The wording is in the file next to each field and **is Shimon's to approve.**
>
> **⚠️ The phone case again, same as the bar hover.** Hovering shows the note on a mouse, but on a
> touch screen a tap opens it and it stays open, and a tap anywhere else closes it. Escape closes it
> too, and it works from the keyboard. Verified: hover opens and closes, tap pins it open, tap away
> closes, tapping a second question mark switches to it, Escape closes. **Nobody can end up stuck
> with a note they cannot dismiss.**
>
> **Two details worth keeping if this is rebuilt.** The visible dot is 17px so it stays subtle, but an
> invisible pad around it makes the tappable area about 35px. And each explanation lives in a
> visually hidden span next to its button, so a screen reader reads it even with no JavaScript, and
> the visual note is filled from that same text rather than duplicating it.

> **➡️ REVISION 7, 2026-08-27 — the ranges opened up, and the design snapshotted.**
>
> **Years now go to 120** (was 50) and **rate of return to 100%** (was 30), in both the input and the
> code that clamps it.
>
> **⚠️ Three things genuinely broke at the new extremes and were fixed. Do not undo these.**
> At the top of both ranges the result is about **10 to the power of 54 dollars**, which printed out
> as a 71 character number.
> - **Number formatting.** Anything from a quadrillion up now shows in short form (`$7.76e53`)
>   instead of seventy digits, and the chart's side labels understand billions and trillions rather
>   than stopping at millions.
> - **The headline shrinks to fit** rather than spilling out of its panel. It measures itself and
>   steps the type size down until it fits, so no figure can overflow at any screen size.
> - **Pointing at the chart was rebuilt.** It used to place one invisible hit area per year. At 120
>   years each is under 2px wide, which is untappable on a phone. There is now **a single overlay
>   that works out the year from where the pointer is**, so it behaves the same with 10 bars or 120.
>   Verified: **all 120 years are reachable**, sweeping the full width of the plot. Arrow keys step
>   through the years for keyboard users, and Escape closes.
>
> **The honest limitation to repeat if he asks.** At 120 years on a phone each bar is under 2px, so
> the chart reads as a filled growth curve rather than 120 separate bars. That is a physical limit of
> the screen, not a bug. Pointing still names the exact year, and **the table view gives every year's
> figures**, which is what dense data is for. Nothing was capped or hidden to work around it.
>
> **Checked at both extremes** at 375px and 1200px: 120 years at 4%, 50 years at 100%, and the full
> 120 years at 100%. In every case the figure fits, the page never scrolls sideways, the side labels
> stay sensible, and the table stays inside its own scrolling frame.

> **A real bug was caught and fixed while testing this revision:** the wide table made the whole page
> scroll sideways on a phone instead of scrolling inside its own box. Cause was the default
> `min-width:auto` on a grid child. Fixed with `.calc>*{min-width:0}`, and re-tested at 375, 414, 768
> and 1200 pixels: the page no longer moves sideways at any width and the table scrolls within its
> own frame. **Watch for this on every future calculator that has a table.**

---

### 18. Calculators 3 and 8 — the two tax ones

**Added:** 2026-08-27 · **Scope cut by Shimon 2026-08-27** — he originally asked for six tax
calculators and then cut it to two

Two tax calculators, numbered 3 and 8. **The numbers stay as they are** — 8 is not being moved down
to 4 just because the ones in between were dropped. See the
[calculator numbering](#calculators--the-permanent-numbering) section.

- **Calculator 3** — S-corp vs LLC savings
- **Calculator 8** — late filing and payment penalties plus interest

**Not started.** He asked to see calculators 1 and 2 first and judge how simple they feel, so the
tone is settled before either of these is built.

**Why it matters:** these are tax calculations with the firm's name on them. A wrong number here is a
different kind of problem from a wrong number on a savings calculator — a visitor could act on it,
and the firm is a regulated practice. **Neither gets published without Shimon checking the figures.**

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon's request
> 2026-08-27, cut to two the same day.*
>
> **Wait for his verdict on 1 and 2 before building either of these.** That was his explicit
> instruction: he did not want a batch built and then to discover the tone was wrong.
>
> **⚠️ The rule that matters most on both.** They must be right and current for the **2026 tax
> year**. Where a genuine answer depends on facts a normal visitor cannot supply — their state, their
> filing status, their other income — **say so on the page rather than quietly picking a value.** A
> silent assumption that produces a confident wrong number is the failure mode to avoid here; an
> honest "this depends on X, talk to us" is not a worse calculator.
>
> **Where that bites on each:**
> - **Calculator 3 (S-corp vs LLC)** turns on a *reasonable salary*, which is a professional
>   judgement rather than a figure a visitor knows, and the answer also moves with state tax and the
>   Social Security wage base. Expect to show the salary as an adjustable input with a plainly
>   labelled default, and to say on the page that the real figure is a judgement call.
> - **Calculator 8 (penalties and interest)** depends on the IRS underpayment interest rate, which is
>   **reset every quarter** — so whatever rate is used has to be shown on the page with its date, or
>   it silently goes stale. Failure-to-file and failure-to-pay are separate penalties that interact
>   (the file penalty is reduced in months where both apply), and there is a minimum penalty for
>   returns over 60 days late. Get the interaction right or the number will be wrong in the common
>   case.
>
> **Both are subject to the same simplicity brief** recorded under the numbering section.

---

### 19. The footer's Resources list doesn't include Financial Calculators

**✅ DONE — LIVE 2026-09-15, commit `68b9eda`.** Added to the footer on all 17 pages, **directly under Due Dates**, which is where he asked for it.

**Added:** 2026-09-02 · *found in the verification of the calculator work*

The Resources menu at the top of every page now lists three things — Track Your Refund, Due Dates and
Financial Calculators. The Resources column at the bottom of every page lists only the first two.
Same on all fifteen pages.

Nothing is broken. Every page is still reachable, and the top menu is the one most visitors use. But
the two lists disagree, and someone who scrolls to the bottom looking for the calculators won't find
them there.

**Why it matters:** small on its own. It grows with every calculator added — the gap between the two
menus widens each time rather than staying the same size.

**This is a decision, not just a fix.** The footer list was never a copy of the top menu — it also
carries Client Login, About and Contact, which the top Resources menu doesn't. So "make them match"
isn't obviously the right answer. Shimon's call.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: verification 2026-09-02,
> checked against the live site and against the committed files at `66d8bac`.*
>
> **What the two lists actually contain**, identical on all 15 pages:
> - **Header dropdown** (`nav.nl .drop .dmenu`): Track Your Refund · Due Dates · Financial Calculators
> - **Mobile menu** (`#mmenu .msub`): identical to the header dropdown — the calculators entry is
>   present and correct there. Verified by opening the menu on the live site.
> - **Footer column** (`.fcol` under `<h5>Resources</h5>`): Client Login · Track Your Refund ·
>   Due Dates · About · Contact
>
> **The footer is not a mirror of the dropdown and never was** — it is a wider "everything else"
> column that predates the calculators. **Do not present this to Shimon as a bug introduced by the
> calculator work; it wasn't.** Commit `626d9ab` added the entry to the header and mobile menus on all
> 13 existing pages and left every footer untouched deliberately. The diff against `4fd195e` confirms
> the footers are byte-identical to before the calculator work — the only lines that changed on those
> 13 pages were the two menu entries.
>
> **What would close it.** One `<a href="calculators.html">Financial Calculators</a>` inside the
> Resources `.fcol`, on all 15 pages, with `../calculators.html` on the six service pages. It
> lengthens that footer column by one line on **every page of the site**, so it is a visible change
> everywhere: **Rule 2 — preview it before building it.**
>
> **The alternative he may prefer** is to leave the footer as the short "everything else" list and
> accept the top menu as where resources live. That is a legitimate answer and it requires touching
> nothing.

---

### 20. The working notes are not backed up anywhere

**Added:** 2026-09-02 · *found in the verification of the calculator work*

Five things live only on Shimon's computer: this to-do list, the decisions record, the audit
instructions, the gate file that tells Claude how to work here, and the settings folder. None of them
are saved anywhere else.

The website itself is safe — every page is backed up online and matches what's published. It is only
the notes that aren't. If the machine died tomorrow the site would survive and the notes would not.
This list alone is over 2,600 lines built up over weeks.

**Why it matters:** this file exists precisely because Claude forgets between sessions. It *is* the
memory. Losing it loses the reasoning behind every decision made on the site — not just the list of
work still outstanding.

**⚠️ The obvious fix is the wrong one.** Saving these files online the same way the web pages are
saved would publish them at his web address, where anyone could read them — and this list contains
the security findings. The notes need somewhere private, not somewhere public. The options are in the
block below. **This is his decision, and it should not be actioned without him choosing.**

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: verification 2026-09-02.*
>
> **The five untracked paths:** `CLAUDE.md`, `TODO.md`, `DECISIONS.md`, `AUDITS.md`, `.claude/`.
> `git status` reports them untracked; `git ls-files` confirms the repository tracks only the 15 HTML
> pages, `assets/`, and `.nojekyll`.
>
> **🔒 They were left untracked on purpose — do NOT "fix" this by committing them.** The site is
> served from the repository root, so every tracked file is published verbatim at the web address.
> There is **no `.gitignore` and no `vercel.json`** in the repo, so nothing currently filters what
> gets served. Confirmed on the live site 2026-09-02: `/assets/site.css` returns **200**, while
> `/TODO.md`, `/DECISIONS.md`, `/CLAUDE.md` and `/AUDITS.md` all return **404** — they are absent
> precisely *because* they are untracked. Commit them as they stand and they become **publicly
> readable**, and `TODO.md` carries the full standing audit including the security findings and the
> domain situation. That is a worse outcome than the backup gap, which is why the earlier session left
> it alone.
>
> **The options, for him to choose between — do not pick one for him:**
> 1. **A second, private repository** holding just the notes, separate from the published one. Keeps
>    them versioned and off the website entirely. Most robust; means two repositories to keep straight.
> 2. **Move the notes out of the website folder** into one that is already backed up. This already has
>    precedent — the rulebook lives in the app's repository for exactly this reason. Fits the existing
>    pattern; the relative links between these files would need re-checking afterwards.
> 3. **Commit them here but stop them being served**, with a `vercel.json` that refuses those paths.
>    Simplest to set up and keeps everything in one folder, but it makes the privacy depend on a
>    config file staying correct forever — one mistake, or one future host change, republishes them.
>    Fragile in a way the other options are not.
> 4. **Plain file copy** to a backed-up location, no version control. No history, and it drifts out of
>    date the moment someone forgets to re-copy it.
>
> **Orthogonal to whichever he picks:** a `.gitignore` listing these paths would stop them being
> committed to the published repo by accident — including by a future Claude that never read this
> block. Worth raising with him alongside the choice; it is not itself one of the four options.

---

### 21. A black box appears around the whole chart when you hover over it

**✅ DONE 2026-09-03 — shipped in commit `d412475`, live and checked.** Clicking the chart now does
nothing at all; hovering still highlights a year and clears when the pointer leaves. The black box is
gone.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

> **What it turned out to be — the diagnosis in the block below was right, and worth keeping.** There
> was **never a click handler.** Clicking gave the transparent overlay *focus*, and that did two
> things at once: the `focus` handler lit a year and left it lit, and the browser drew its default
> ring around the overlay — which spans the whole chart, hence a box round all of it. The "lock" and
> the "black line" were one mechanism, not two.
>
> **The fix, as shipped:** the ring is suppressed on `:focus` and restored on `:focus-visible`, and
> the focus handler highlights only when the focus came from the keyboard. A fallback watches whether
> the last input was Tab or a pointer, for browsers without `:focus-visible`.
>
> **Checked on the live page 2026-09-03:** a click shows nothing and draws no outline
> (`outlineStyle: none`); hovering highlights the year and dims the other 18 segments; the pointer
> leaving clears it; a tap still shows the year at 375px with no sideways scroll; the arrow keys still
> step through the years; no console errors. Both CSS rules are present and parsed on the live page,
> and `2px solid var(--gold-d)` computes there to `rgb(124, 90, 34)` — the firm's gold. **Nothing else
> changed:** the other 14 pages and `assets/site.css` are byte-identical, and the default result is
> still $29,542.
>
> **The keyboard ring was confirmed with a real Tab press on a local copy, not on the live page** —
> the browser pane would not deliver a Tab keystroke to the live tab. The live check proved the rule
> and the colour resolve correctly; it did not watch the ring appear. Worth one look on a real
> keyboard if it ever matters.

**Added:** 2026-09-02 · *reported by Shimon*

In his words: on the compound interest calculator, when hovering over a bar, **the whole chart gets
surrounded with a thick black line.** He doesn't like that black box around it.

**Why it matters:** it happens during ordinary use, on the one page on the site built to be played
with, and it looks like something is broken rather than deliberate. Every other control on that page
already lights up in the firm's gold when you use it — this is the one that doesn't.

**Not a five-second deletion, and worth knowing why.** That outline is the browser's way of showing
where you are on the page, and somebody using the keyboard instead of a mouse genuinely needs it. So
it can't simply be switched off. The fix is to hide it for mouse users and keep it for keyboard
users — a normal thing to do, but it is two changes rather than one, and it needs checking both ways.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon, 2026-09-02.
> **Diagnosed from the source, not visually reproduced** — the browser pane available at the time
> could not composite frames, so no screenshot was taken and the focus ring was not seen. Confirm on
> a real browser before acting.*
>
> **Almost certainly the default focus ring on the chart's interactive overlay.**
> `compound-interest-calculator.html` **L325** draws a single full-width `<rect fill="transparent"
> tabindex="0" role="img" aria-label="Balance for each year. Use the left and right arrow keys…">`
> across the whole plot area — the variable `plot`. Because that one element spans the entire chart,
> a focus ring on it reads exactly as Shimon describes it: a box around the whole chart, not around
> the bar under the pointer.
>
> **Why it fires on the mouse and not just the keyboard.** `plot` carries
> `mousemove` (L365) alongside `focus` (L369) and `blur` (L370). A `tabindex="0"` element takes focus
> on mouse interaction as well as on Tab, so the ring appears during ordinary hovering and clicking.
>
> **The actual gap: this element was missed when the rest of the page was styled.** Every other
> control on the page defines its own `:focus-visible` in the page's `<style>` block —
> `.qm` (L36), `.inp input` (L49), `.freq input` (L56), `.vtabs button` (L76) — all
> `outline:2px solid var(--gold-d)`. **`#chart` and its overlay have no focus rule at all**, so they
> fall through to the browser default, which is a thick dark ring. That is the black box.
>
> **What would close it.** A rule pair scoped to the overlay: `outline:none` on `:focus`, and the
> gold `outline:2px solid var(--gold-d)` on `:focus-visible`, matching the four controls above.
> `:focus-visible` is precisely the selector that distinguishes keyboard from pointer, so this keeps
> the keyboard affordance the aria-label promises while removing the box he is seeing.
> **Test both ways before calling it done:** hover and click with a mouse (no ring), then Tab to the
> chart and use the arrow keys (gold ring, and the year readout still steps).
>
> **⚠️ Do not "fix" this by removing `tabindex` or the aria-label.** That would delete the keyboard
> access rather than the outline, and the label explicitly tells a screen-reader user the arrow keys
> work. Rule 7 territory: the page would then be telling people something untrue.
>
> **Visual change — Rule 2 applies.** It is small and only visible mid-interaction, but it is a
> change to how the site looks. Preview it.

---

### 22. A third view on the compound interest calculator — a graph

**✅ DONE — APPROVED AND LIVE 2026-09-15, commit `df9c046`.** Built into the real calculator page from the mockup: same shell, same shared stylesheet, third icon in the existing toggle. **The mockup file itself was not shipped.** What went live is exactly what he approved — two lines, no crossing marker, no dots at rest, and a hover box of figures only.

`C:\Users\Admin\Documents\outputs\compound-interest-graph-view-mockup.html`

**He redirected this after seeing the first version.** In his words: *“I want line 1. Principle 2. Interest so at one point it crosses”* — and he sent a reference showing a Total principal line against a Total interest line, each shaded, crossing partway along. The first mockup drew the balance against the principal, which can never cross. **The rebuilt one draws total principal against total interest, which does.**

It adds a third icon to the toggle, beside the bars and the table. Pointing anywhere on it gives the year, the two running totals and the balance they add up to. **Nothing is drawn on the chart to mark where the lines cross** — they simply cross.

**He then sent a second reference — the same chart from the same tool, but showing the hover box.** It is not a different idea, it is the first one from another angle: what he had not shown the first time was what happens when you point at the chart. Folded in from it: the hover box laid out as a heading with a rule under it, **a colour patch beside each name** matching its line, and **a bold Total balance row at the bottom, ruled off** — the two figures and the sum they make. Pointing lights up the year: a faint vertical line and a dot on each line. *(The reference also puts a dot on every year of the line; he has since taken those off — see below.)*

> **The two references do not conflict with each other. The conflict is between the second one and this site.** The reference's hover box is a white card; the calculator's own hover box, on the bar view of the same page, is dark. **I followed the site, not the reference** — the same call already made over its blue and green, which became his gold and tan. Switching views should not change what the hover box looks like. **If he wants the white card, it is a small change, but it should be made to both views on the page, not one.**
>
> **✅ HE STRUCK BOTH OF THE THINGS THAT WERE MINE, 2026-09-15.** In his words: remove *“the marker line on the crossover year … he just doesn’t want it annotated”*, and *“remove the description text from the hover box. Keep the figures, drop the wording around them.”* Both are gone: the dotted line, the dot and the words *interest pulls ahead* are off the chart, and the hover box is now the three rows of figures and nothing else. **Do not put either back.** He was shown them, he looked, he said no.
>
> **He then asked a third time for the same thing, in different words:** *“remove the interest ahead/behind line from the hover box … just the figures, nothing interpretive at all.”* **That was the same line as the “description text” above and was already gone** — no further change was needed. Worth knowing because it shows what he is after: **the hover box states figures and does not interpret them.** Anything added to it later should meet that test.
>
> **✅ SETTLED 2026-09-15. THE SENTENCE UNDER THE CHART STAYS. DO NOT REMOVE IT.**
>
> He asked a second time to *“take the line off the graph that marks the year interest pulls ahead”*, so the rendered chart was gone through element by element rather than read off the source. **Every single thing it draws at rest:** four gridlines, four money labels, ten year labels at even three year steps, two shaded areas, two lines, and three pointer markers sitting at `opacity="0"`. **There is nothing at the crossing year that is not at every other year** — the marker really had gone the first time.
>
> What was left naming the crossing was the **line of text under the chart** — *“From year 30 onwards the interest you have earned is worth more than everything you have paid in.”* Removing it was started, and he stopped it mid way: **“Leave that line”**, then **“Its good now”**. So it stays, and the chart stays bare.
>
> **For whoever picks this up next:** if he says it again, the thing to look at is that sentence, not the chart — the chart has been proved clean twice. Check as well that he is not looking at an older copy of the file, since every version has been written to the same path.
>
> **✅ NO DOTS ON THE LINES AT REST — his instruction, 2026-09-15.** In his words: *“No dots on the lines at rest. The year markers should only appear when hovering — plain lines otherwise, and the dot appears on the point you’re pointing at.”* The lines are now drawn plain. Every year’s position is still worked out and kept, because that is what the two pointer markers are placed from. **Do not put the resting dots back**, and note this also retires the old rule about dropping them when the years got too close together — there is nothing left to drop.
>
> **The hover box is smaller on a phone.** At full size it covered nearly the whole chart on a 375px screen, which defeats the point of pointing at it.

> **⚠️ THE ONE THING HE MUST SEE: on the figures the page opens with, the lines do not cross.** $5,000 to start, $150 a month, 4%, 10 years gives **$23,000 put in against $6,542 earned** by year 10. At 4% the crossing is **year 30**, well past the end of the chart. So the view opens on a picture that does not show the thing it was built to show.
>
> **The defaults were not changed to make it look better.** He was told instead, and the view says so itself: when the lines have not crossed, a line under the chart reads *“The two lines have not crossed yet … at this rate the interest would overtake what you put in around year 30.”* The crossing year is worked out by running the same figures further forward; **nothing drawn on the chart, and no figure quoted anywhere, goes beyond the years he asked for.** When the crossing does fall inside the years shown, the line underneath names it instead.
>
> **If he wants the crossing visible when the page opens, that is a decision about the default figures, and it is his to make** — not something to quietly change. Holding everything else as it is: 5% crosses at year 23, 6% at 19, 7% at 16, 8% at 14. Raising the years of growth would do it just as well.
>
> **✅ THE “WHICH KIND OF GRAPH” QUESTION IS NOW ANSWERED AND CLOSED, 2026-09-15.** He said which two lines he wanted — principal and interest, so that at some year they cross — he was shown it, he had it stripped back three times, and he approved it. **It is built and live.** There is nothing left open here.
>
> **Nothing in the new view is focusable** — no tabindex, no click handler, pointer and touch only, the rule set after the black box.
>
> **Colours follow the bar chart deliberately:** principal in the same gold and interest in the same tan, so a figure does not change colour when he switches views. The reference used blue and green; his brand does not.
>
> **Checked:** the figures on the chart match a separate model built from scratch, to the dollar, including the crossing year. The three views switch cleanly, the line redraws when the figures change and when the window resizes, the bars and the table still work, nothing is focusable, and at 375px there is no sideways scroll, the marker label stays inside the chart and all three icons are 44px tall.
>
> **One bug found and fixed in the rebuild:** the line view was measuring the width of the bar chart's box, which is hidden while the line view is showing, so it measured nothing and fell back to a default width. On a phone that meant the chart was drawn for a wider screen and scaled down. It now measures its own box.

**Added:** 2026-09-02 · *reported by Shimon*

In his words: on the compound interest calculator he wants **another view, a graph.** There are
currently bars and a table; he wants a graph as a third view.

**⚠️ One thing to settle with him before anything is built:** he said "graph", and that most likely
means a **line showing the balance rising over time**, as opposed to the year-by-year bars already
there. **But he did not say so, and it should not be assumed.** "Graph" could equally mean a pie of
principal against growth, or an area chart, or something else he has in mind. **Ask him which he
means before building it** — it is one question, and building the wrong one wastes his time reviewing
it as well as the work itself.

**The mechanism already exists**, so this is smaller than it sounds: the chart header already carries
a little toggle that switches between the bars and the table. A third view slots into the same
control rather than needing anything new.

**Why it matters:** it is the first thing he has asked for on the calculator since it went live, and
he asked for it unprompted — so he is using it.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon, 2026-09-02.*
>
> **Where it goes.** `compound-interest-calculator.html`. The toggle is `.vtabs` in the `.vhead`
> block, holding two buttons — `#vChart` and `#vTable` — wired at the foot of the script to
> `setView(true)` / `setView(false)`, which show and hide `#paneChart` and `#paneTable` and set
> `aria-pressed` on each button. **A third view means `setView` stops being a boolean.** Expect to
> change it to take a view name and drive three panes, rather than bolting a second flag alongside
> the first.
>
> **The toggle currently holds two icons and will need a third.** Each button carries an inline SVG,
> an `aria-label` and a `title` — the bar-chart glyph and the table glyph. A third needs a glyph in
> the same 24×24 stroked style, plus its label. **Check the width at 375px:** the toggle sits on the
> same row as the view title, and the row was measured tight on a phone when the calculator was
> built.
>
> **The data is already there — no new maths.** `rows[]` already holds, per year: `year`, `start`,
> `addY`, `cumAdd`, `intY`, `cumInt`, `balance`. A balance-over-time line needs `year` and `balance`
> and nothing else. **Do not recompute anything** — the arithmetic is settled and verified, and item
> 16's block records how it was checked.
>
> **Drawing convention to match.** The existing chart is inline SVG drawn in plain JavaScript with no
> library, into `#chart` with a `viewBox`, and it is redrawn by `draw()` on every recalculation. A
> third view must follow the same approach — **do not introduce a charting library** for this; the
> page currently fetches nothing and works offline, and that is deliberate.
>
> **Two behaviours the current chart has that a new one will be expected to match:** the hover
> readout with the year's figures, and the keyboard arrow-key stepping. Whether the line view needs
> both is worth asking him rather than assuming — but if it has a hover readout, it should behave the
> same way the bars do, and **clicking must do nothing**, per item 21.
>
> **Rule 2 applies squarely — this is a new visual thing on the page.** Build a standalone preview
> and get his approval on the look before touching the live page.
>
> **📌 The "which kind of graph" question stays OPEN — he will answer it when we come to build it.**
> Confirmed 2026-09-03: he does not want to settle it now. **Do not assume, and do not pick one to get
> started.** Ask him at the point of building, not before.

---

### 23. Retirement calculator — calculator 9

**Added:** 2026-09-02 · *reported by Shimon* · **Numbered 9** — see the
[calculator numbering](#calculators--the-permanent-numbering) section

In his words: a calculator that works out **how much you need to put away, and how much you'll have by
retirement.**

The inputs he described, roughly: what you earn now, what percentage of it you are putting away or
should be putting away, what you would have by retirement, and how long you could live off it. His
example of that last part was **drawing 5% a year while it grows at 10%.**

**⚠️ The details are not settled and must be worked through with him before this is built.** What he
gave is the shape of the thing, not a specification. The list above is his sketch, recorded as he said
it — it is not a finished set of inputs, and several of the pieces interact in ways that need his
decision rather than a guess.

**Why it matters:** it is the first calculator he has asked for that is about a person's own money
over a whole working life. The numbers it produces are the kind someone might actually plan around,
which puts it closer to advice than the compound interest one.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon, 2026-09-02.*
>
> **Numbered 9.** Next free number at the time of writing; 4 to 7 are retired, 8 is taken. The
> numbering rules in the registry apply — **the number never appears anywhere a visitor can see it.**
>
> **What needs settling with him before a line is written.** These are genuine forks, not details to
> be tidied later:
> - **Is the salary percentage an input or an output?** He described both "what percentage you're
>   putting away" *and* "should put away". Those are two different calculators: one takes a
>   contribution rate and shows the result; the other takes a target and works backwards to the rate
>   needed. It may want to be both, but that is his call.
> - **The drawdown half is a second calculation, not a footnote.** "How long you could live off it"
>   with 5% drawn against 10% growth is a separate model bolted onto the accumulation one — and at
>   those figures the pot grows indefinitely, so the honest answer is "it does not run out", which may
>   not be what he expects to see. **Worth showing him that specific case early.**
> - **Does it assume the salary rises?** A contribution set as a percentage of pay behaves very
>   differently with and without pay growth, over thirty years.
> - **Retirement age, or years to retirement?** And is there an existing pot to start from?
>
> **⚠️ The accuracy and advice constraint bites harder here than on calculator 1.** A savings-growth
> figure is arithmetic. A retirement number is the thing people make decisions about, and a **10%
> growth assumption is optimistic enough that it should not be a silent default.** The firm is a
> regulated practice and does not give investment advice — `terms.html` says the site is general
> information only. Expect the disclaimer to need to work harder than calculator 1's, and **expect
> Shimon to have to approve its wording** before anything is published. See item 16's block for how
> that was handled the first time. Rule 7.
>
> **Reuse what exists.** Calculator 1 already has the compounding maths, the chart, the table, the
> year-by-year `rows[]` shape, and the input styling. This should look like a sibling of it, not a new
> design.

---

### 24. Change the description on the compound interest calculator

**✅ DONE 2026-09-03 — shipped in commit `b8e0153`, live and checked.** He supplied the text and it
was used character for character. The line under the page heading now reads: *"Estimate your savings
or spending through our compound interest calculator. Enter your initial amount, contributions, rate
of return and years of growth to see how your balance increases over time."*
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

> **Which text it turned out to be:** the line under the page heading in `.phero` — one of the three
> candidates the block below flagged. **The other two were NOT changed and are still the old wording:**
> the `meta`/`og`/`twitter` descriptions still read *"Work out what your savings could grow to over
> time, with regular contributions."*, and the card on `calculators.html` still reads *"See what your
> savings could grow to over the years."* He did not ask for those, so they were left alone. **If he
> ever wants the link-preview text to match the page, that is a separate change touching four places
> plus the card.**
>
> **Verified before pushing, on the live page, by swapping the text in a browser session only.** It is
> much longer — 197 characters against 44 — so it occupies more room: **three lines instead of one at
> 1280px, six instead of two at 375px.** It stays inside its own 620px column, does not overflow its
> parent, wraps with a normal rag (last line 171px of 323 at phone width, not an orphan), and adds no
> sideways scroll at either width. **The hero is 59px taller on a desktop and 118px taller on a
> phone**, which moves the first input down by the same amount.
>
> **🔒 Nothing was adjusted to compensate, deliberately.** Shimon's instruction was to tell him rather
> than work around it. The extra height is the arithmetic of a longer paragraph, not a styling change.
> **If he later wants that height back, the fix is shorter words or a change to `.phero` — do not
> silently shrink the type.**
>
> **Proof the change was only the text:** with the paragraph masked out, the file is byte-identical to
> `808f119`, and the `<style>` and `<script>` blocks hash the same before and after. The other 14 pages
> and `assets/site.css` are byte-identical to `66d8bac`. No console errors.

**Added:** 2026-09-02 · *reported by Shimon*

He wanted the wording on the compound interest calculator changed. **He had text in mind, taken from
MoneyGeek, and supplied it on 2026-09-03.**

**Why it matters:** small, and entirely blocked on him. Worth keeping on the list so it is not
forgotten between now and when he sends it.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon, 2026-09-02.*
>
> **Which text he means is not yet pinned down.** The page currently has three candidates for
> "the description", and he did not say which: the line under the page heading (*"Fill in your
> figures, then press Calculate."*), the `<meta name="description">` and the matching og/twitter
> descriptions (*"Work out what your savings could grow to over time, with regular contributions."*),
> and the card text on `calculators.html` (*"See what your savings could grow to over the years."*).
> **Ask which when the text arrives** — it may well be more than one.
>
> **⚠️ If it is the meta description, it lives in four places on that page** — `meta description`,
> `og:description`, `twitter:description` — and the card on `calculators.html` is a fifth. Change them
> together or the link preview stops matching the page.
>
> **Do not copy MoneyGeek's wording verbatim into the site.** He is taking the text *from* there as a
> model; lifting a competitor's copy onto a regulated firm's public site is a different thing. Use
> what he sends, and if what he sends is a straight copy, say so once and let him decide.
>
> **The disclaimer is separate and is not this.** The estimate-not-advice paragraph was approved
> content — do not fold it into a wording change. See item 16's block.

---

### 25. Every calculator page needs explanatory content underneath it

**Added:** 2026-09-02 · *reported by Shimon*

In his words: under the compound interest calculator there should be a section **explaining how
compound interest works and how it's calculated** — and **the same for every other calculator.** The
point is that the page should be **more than just the calculator.**

**This is a standing requirement, not a one-off.** It applies to the calculator that is live now, and
to every calculator built from here on. A new calculator is not finished until it has its explanation.

**Why it matters:** two reasons, and the second is the one that pays. A visitor who does not already
understand compounding gets a number with no meaning attached — the explanation is what turns it into
something useful. And a page with real substance on it is a page that can be found in a search and
read by someone who was not looking for the firm, which a bare calculator cannot do.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon, 2026-09-02.*
>
> **🔗 This overlaps I18 ("Add an insights or articles section") and it is the same instinct.** I18
> stays where it is as the broader idea; **this item is the specific, narrower thing he actually
> asked for** — explanation on the calculator page itself, not a separate articles section. Do not
> treat them as two separate pieces of work, and do not re-pitch I18 as if this had not been asked
> for. If the explanations are written well they may make I18 unnecessary, or may become its first
> entries.
>
> **Where it goes on the page.** Below the calculator and below the estimate-not-advice line, inside
> the existing `.detail` section. `.note` already exists in `assets/site.css` as a bordered cream
> panel and is the obvious shape for it — **check with him rather than assuming**, since he may want
> plain prose rather than a boxed panel.
>
> **⚠️ Rule 7 applies with real force here — this is explanatory writing published by a regulated
> practice.** "How compound interest is calculated" is a factual claim about arithmetic. It must be
> correct, it must match what the calculator on the same page actually does, and **that includes the
> conventions**: the calculator compounds monthly, and in annual mode treats the contribution as
> going in at the **end** of each year. An explanation that describes plain annual compounding would
> contradict the tool sitting directly above it. Item 16's block records those conventions — read it
> before writing a word.
>
> **Length and tone: this is not a blog post.** The site's voice is short, plain and unhurried. A few
> tight paragraphs and a worked example beat an essay, and Shimon will not read a long draft.
>
> **Rule 2 applies** — it changes the shape of the page. Preview it.

---

### 26. The calculator cards should be a graphic, not words

**✅ DONE, LIVE 2026-09-24, commit `b34c761`.** The whole Financial Calculators page is redesigned (direction C, bold dark). Each card now leads with one large gold drawing on a dark panel, with **no small icon in the corner**. The page has a proper header, a "Before you start" section and a closing panel showing the phone number and email. He approved it as shown: *"perfect, push live."* Checked live at desktop and phone width. **The page's new wording was Claude's draft, approved by him as shown; DECISIONS.md lists it line by line.**
*The notes below are from before it shipped. Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

**✅ FOLLOW-UP DONE, LIVE 2026-09-24, commit `62492e1`.** He rejected the dark header as not matching the rest of the site and picked **H2**, the same layout lightened: cream band with the chart pattern in pale gold. The cards, "Before you start" and the dark closing panel are unchanged. Checked live at desktop and phone width. The history of how he got there:
**🟡 FOLLOW-UP, 2026-09-24, after it went live.** His words: *"the black header background is too much, doesn't match with the rest of the site. The cards are good."* **The cards stay exactly as they are; only the dark header band is to change.** Three light header mockups in `C:\Users\Admin\Documents\outputs\`: `calculators-header-H1-site-cream.html` (the other pages' cream band, chart pattern dropped, logo watermark instead), `calculators-header-H2-cream-with-chart.html` (live layout on cream, chart redrawn in pale gold, cards still overlap), `calculators-header-H3-deeper-sand.html` (cream deepening to sand, centred, gold rule and gold bottom edge, chart dropped because it sat behind the centred title). Pictures are `calc-header-H*-desktop/phone.png`. **Claude's view on the dark closing panel: it still works**, because it matches the cards' dark panels. **Not changed; he has not been asked yet.**

**Added:** 2026-09-02 · *reported by Shimon*

In his words: right now each card on the Financial Calculators page is **a name plus a description
with a small logo in the corner.** He wants it to be **primarily a large graphic or icon with the
calculator's name — not words.**

**⚠️ He wants to confirm the exact treatment before it is built.** He has described the direction, not
the design. **Do not build a version and show it as finished** — Rule 2 exists for precisely this, and
he has said outright he wants to agree the treatment first.

**Why it matters:** the page exists to send people into the calculators, and it will hold four or more
of them before long. A row of near-identical text blocks is harder to scan than a row of distinct
pictures, and this is one of the few pages on the site whose only job is to be chosen from.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon, 2026-09-02.*
>
> **What is there today**, on `calculators.html`: one `<a class="card reveal">` per calculator inside
> `.cgrid`, containing a `.ci` icon block (a 24×24 stroked bar-chart SVG), an `<h3>` with the name, a
> `<p>` of description, and a `.more` line reading "Open calculator →". The `.cgrid` rule is defined
> in that page's own `<style>` — `flex:0 1 340px;max-width:340px` — and was written deliberately to
> wrap cleanly at one, two, three and four cards.
>
> **The `.card` class is shared with the six service cards on the home page.** Restyling `.card`
> itself in `assets/site.css` would change the home page too. **Scope any change to `.cgrid .card` in
> the calculators page's own style block** — the same way `.cgrid` already is.
>
> **The questions to put to him before building** — this is what "confirm the treatment" means:
> - **How big, and drawn how?** A large line icon in the firm's gold, a filled illustration, or a
>   photograph? The site currently uses stroked line icons everywhere and no illustration at all, so
>   an illustrated style would be a new visual language for the site, not just a new card.
> - **Does the description go entirely, or move?** He said "not words", but a name alone gives a
>   first-time visitor no idea what "Compound Interest" will do for them.
> - **Does the "Open calculator →" line stay?** It is the only affordance saying the card is clickable.
> - **One graphic per calculator, meaning four to draw**, not one generic image reused.
>
> **Check it at 375px.** Large graphics are exactly where a phone layout goes wrong, and cards stack
> to full width there.
>
> **Rule 2, emphatically. Standalone preview, his approval, then build.**
>
> **🟡 2026-09-24: THREE MOCKUPS BUILT FOR HIM TO COMPARE. NOTHING CHOSEN, NOTHING BUILT ON THE SITE.**
> His words on the live page: *"it looks very blah now."* In `C:\Users\Admin\Documents\outputs\`:
> `calculators-direction-A-picture-tiles.html` (large gold line drawing on a cream panel, description
> kept), `calculators-direction-B-medallions.html` (dark circles like the home page's numbered steps,
> name only, no description), `calculators-direction-C-preview-panels.html` (dark panel showing the
> shape of the chart each calculator draws, description kept). Each has a 3/4/5/6 switch (`?n=5` in the
> address) and matching `calc-*-desktop/phone(-six).png` pictures. Cards 4 to 6 are the planned
> Retirement, S-corp vs LLC and Penalties & Interest, marked as placeholders. All new styling uses new
> class names, so building any of them leaves the home page's `.card` alone. Icons for all six are
> drawn and live in the mockup files. **When he picks, ask whether the description stays** (B drops it).
>
> **🟡 2026-09-24, same day: BRIEF WIDENED TO THE WHOLE PAGE.** His words: *"Not only the cards, the
> whole page is too plain."* Three whole-page mockups, each built on one of the card directions above:
> `calculators-page-A-warm-editorial.html`, `calculators-page-B-home-page-echo.html`,
> `calculators-page-C-bold-dark.html`, with `calc-page-*` pictures. They add a proper header area, a
> privacy / "estimate, not advice" section, and a closing section with a way to get in touch. **All
> the new wording is Claude's draft, not approved.** It only restates things already true and
> published: the privacy policy's calculator paragraph, "This is an estimate, not advice." from every
> calculator page, and the free call he confirmed. **⚠️ Every "Book a call" button leads to the
> Contact page, whose form sends nothing (item 2).** Phone and email are shown directly in all three
> closing sections for that reason. Adding more buttons that lead to that form compounds item 2.
>
> **🟢 2026-09-24: HE PICKED THE CARD STYLE.** Cards-only direction C, "Preview panels" (the dark
> panels), confirmed from his screenshot. **His two changes:** (1) the dark panel shows the drawing
> from the round medallion version instead of the mini chart; (2) **no small icon in the top corner**:
> one graphic per card. That is the original complaint in this item, so it must not come back. Built
> into whole-page C: `calculators-page-C-bold-dark-v2.html` plus `calc-page-C-bold-dark-v2-*`
> pictures. **The whole-page direction is still not picked**, and the page's new wording is still a
> draft.

---

### 27. Mortgage calculator — ideas from MoneyGeek, for him to pick from

**Added:** 2026-09-03 · *from the mortgage comparison against
`moneygeek.com/loans/mortgage-calculator`* · **Belongs to calculator 2 — see
[item 17](#17-calculator-2--monthly-mortgage-payment)**

Everything MoneyGeek's mortgage calculator does that his draft does not. **He went through this list
on 2026-09-03 and picked.** What follows is what is left.

**✅ PICKED, BUILT AND SHIPPED 2026-09-03** — live in commit `76d83eb`

- Headline figure is the full monthly cost, not just the loan → *question H, answered*
- A full year-by-year payoff schedule, as a third tab beside the chart and the breakdown
- Hovering the bar shows the amount of principal and the amount of interest

**❌ REJECTED BY HIM 2026-09-03 — do not build, do not raise again**

- ~~Down payment as a dollar amount and a percentage, linked both ways~~
- ~~Loan term as a dropdown of 10 / 15 / 20 / 30 years~~ — he likes the buttons as they are
- ~~Monthly or yearly toggle on the tax and insurance figures~~

**⬜ STILL OPEN — not picked, not rejected**

- Property tax entered as a percentage of the home's value
- HOA fees as an input
- Extra monthly overpayment, showing years and interest saved
- Zip code, to localise tax and rate figures
- Payment broken into principal and interest as separate lines
- PMI, added automatically when the deposit is under 20%
- The point where you reach 20% equity and PMI can come off
- Extra fields shown as collapsed "+" rows rather than a block
- An affordability view based on the 28/36 income rule

**Explanatory content — this is [item 25](#25-every-calculator-page-needs-explanatory-content-underneath-it), not a calculator feature**

- The formula written out, so you can do it by hand
- A worked example with real numbers
- Step-by-step "how to use this"
- An FAQ
- Short customer stories showing what the calculator settled

**Also done in the same pass, from his own instructions rather than this list:** "Price of the home"
renamed **Home price**, "Money you're putting down" renamed **Down payment**, and the tax and
insurance fields relabelled **Property tax** and **Home insurance** and set side by side in equal
columns.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: mortgage comparison
> against `moneygeek.com/loans/mortgage-calculator`, 2026-09-03, read in a browser. Updated the same
> day with his picks.*
>
> **✅ SETTLED 2026-09-03 — the down payment field is finished, do not revisit it.** His wording on
> 2026-09-03 was *"Down payment stays a percentage"*, which read ambiguously against a field that is
> actually a **dollar** box with a percentage read-out underneath it ("That's 20% of the price."). It
> was queried and he answered plainly: **leave it exactly as built.** So the settled design is a
> dollar input, with the percentage shown beneath it, and **no linked percentage input** — that
> version he rejected outright. **This is now a decision, not an open question.**
>
> **🔗 Do not treat this as a separate piece of work from item 17.** Item 17 is the calculator; this
> is a list of things it could also do. **Nothing here is approved.** When he picks, the picked items
> become part of item 17's build, not a second project.
>
> **The last five are item 25 and are listed here only so the comparison is complete.** Item 25 is the
> standing requirement that every calculator page carries an explanation. **Do not build them as
> mortgage-only features and do not duplicate them into item 25** — they are the same work seen from
> two directions.
>
> **Two that carry real risk if picked, worth saying before he chooses:**
> - **Zip code to localise tax and rate figures** needs a source of truth for local property tax rates
>   that is kept current. A stale rate on a CPA firm's site is a wrong number with the firm's name on
>   it. Rule 7. This is much bigger than it looks in a one-line list.
> - **PMI** is a rules-based figure that varies by lender and credit profile. Adding it means
>   publishing an estimate of somebody else's pricing. Whatever is shown needs its assumption stated
>   on the page.
>
> **The cheap, safe ones**, if he wants a starting point: the linked dollar/percentage down payment,
> the term dropdown, and the principal/interest split. All three are arithmetic the draft already does
> and would need no new source of data.
>
> **What MoneyGeek's own defaults were** on the day it was read: $250,000 price, $50,000 down (20%),
> 7% rate, 30-year fixed, $158/month property tax, $165/month insurance, PMI $0, HOA $0, headline
> "Total Monthly Payment $1,654" with "Principal & interest $1,331" beneath it. Its three tabs were
> **Monthly Payment / Affordability / Amortization**.

---

### 29. The hover box on two calculators never moves — it sits at the left edge whatever you point at

**🔴 LIVE ON THE SITE NOW. Found 2026-09-15 while building the graph view. Not fixed — his call.**

Point at any year on the **compound interest** chart or the **break even** chart and the little dark box of figures appears with the right numbers in it, but it always appears in the same place, hard against the left edge of the chart. It is supposed to follow your pointer and sit under the year you are pointing at. The figures are correct; only the position is wrong. **The mortgage calculator is not affected.**

> 📎 **CONTEXT FOR CLAUDE**
>
> **The cause, exactly.** In `showYear()` the line that places the box reads
> `Math.min(cx-wr.left-tw/2, wr.clientWidth-tw-4)`. `wr` is the result of `getBoundingClientRect()`, which is a rectangle and **has no `clientWidth`**, so that half of the comparison is `undefined`, `Math.min` returns `NaN`, and `tip.style.left` is set to the string `"NaNpx"` — which the browser rejects, leaving the box wherever CSS put it. It should read **`wrap.clientWidth`**, the element, not `wr.clientWidth`, the rectangle. One word.
>
> **Proved, not guessed:** hovering at 10%, 50% and 90% across the live chart, `tip.style.left` came back as the empty string every time while the year in the box changed correctly from 1 to 5 to 9.
>
> **Where it is:** `compound-interest-calculator.html` and `break-even-calculator.html`, one occurrence each. `mortgage-calculator.html` does not contain the line. The `top` on the same box is computed from `wr.top`, which *is* a real property of a rectangle, so the vertical placement works — which is why this reads as a quirk rather than an obvious fault.
>
> **Already fixed in the graph mockup** (item 22), so the fix is known to work. It has deliberately **not** been applied to the two live pages: they are untouched, and the four fixes from 2026-09-15 are still sitting uncommitted waiting on him. **Do not fold this into that batch without asking** — he approved those four by name.
>
> **Worth telling him plainly:** nothing shows a wrong number because of this. It is a polish problem on a page that is otherwise finished, and it has been live since the calculators shipped.

**Added:** 2026-09-15 · *found by Claude while building item 22, not reported by Shimon*

---

### 30. Give each calculator page a header with some design to it

**Added:** 2026-09-24 · *Shimon's request*

In his words: *"now make the headers on each calculator page better with some sort of design like you did here. send me screenshots."* "Here" is the cream header with the pale chart that went live on the Financial Calculators page the same day.

**✅ DONE, LIVE 2026-09-24, commit `f8c1c55`.** He chose **the pale drawing header over the large medallion**. All three calculator pages now have it, each showing its own card drawing, and each ends with the "Questions about *your results?*" panel. **The panel is light, not dark**, because the dark one competed with the results and chart. The phone number and email are shown as working links. **The maths was proved untouched:** 13 test cases gave identical results before the change, locally, and live after it. Checked live at desktop and phone width. The index's "your results" wording is still flagged and has not been changed.
*The notes below are from before it shipped. Listed in DONE at the foot of this file.*

**(Before it shipped:) TWO DIRECTIONS BUILT, ALL THREE PAGES EACH.**

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Claude's mockups, 2026-09-24.*
>
> **The mockups**, in `C:\Users\Admin\Documents\outputs\`:
> `calc-header-medallion-{compound-interest,mortgage,break-even}.html` and
> `calc-header-pale-drawing-{…}.html`, each with `-desktop.png` / `-phone.png` first-screen pictures.
>
> **What both share:** the cream band, the title on the left with "Calculator" in gold italic (same idea as "Financial *calculators*" on the index), and a small "← Financial Calculators" link above the title back to the index. The intro paragraphs are his existing wording, unchanged. Each page carries **the same drawing as its card**, so a future calculator needs no new design: its card drawing is its header drawing. Drawings for Retirement, S-corp vs LLC and Penalties & Interest already exist in the mockup code.
> - **Medallion:** the drawing in a dark circle on the right, like the round version shown earlier. It stays a real mark on a phone.
> - **Pale drawing:** the drawing large and faint on the right, like the index's pale chart. It is quieter, but has to shrink to a small faint mark on a phone.
>
> **Deliberately different from the index:** there is no chart pattern and no cards overlapping the header, so the index still reads as the parent page.
>
> **Height, measured at 375 wide:** today's header is 385px (compound, break-even) and 415px (mortgage). **Both new headers are shorter on every page**: by 71px on compound, 76px on mortgage and 103px on break-even. So the first input box is higher on the first screen. On desktop nothing moves (first input at 470 versus 471 today). The paragraphs drop from 18px to 15.5px on a phone, which is part of why they are shorter.
>
> **New wording:** only the link label "Financial Calculators", which is the index page's existing name. The styles are scoped to new class names, and the shared `.phero` is not touched.
>
> **Added to the brief the same day, his words: *"and also the book a call box on bottom."*** Every mockup now ends with the "Questions about *your results?*" panel from the index, placed after each page's "estimate, not advice" note. It has the same wording and button, and **the phone number and email shown as working links**, because the Contact page's form still sends nothing (item 2). **On the calculator pages it is a light version**: a white card with a thin gold left edge, on a cream band. It is not the index's dark panel. **Why:** under a light calculator, the dark panel became the heaviest thing on the page and pulled the eye from the result figure; with the medallion header it would be a second dark block too. The gold edge echoes the gold edge on the "estimate, not advice" note just above it. A dark version was built and compared before choosing (scratch only). The pictures are now full-page `-desktop.png` / `-phone.png`, plus `-desktop-first-screen.png` / `-phone-first-screen.png` for the fold.
>
> **⚠️ Flagged, not changed: the index's closing panel reads "Questions about *your results?*"**, but the index has no results on it; it is the page you choose a calculator from. On the calculator pages the line is exactly right. If he wants, the index could say something else. **Do not change the index without his say so.**

---

### 28. Break Even Calculator — calculator 10

**✅ DONE 2026-09-11 — shipped in commit `213dfbb`, live at `break-even-calculator.html`** and
reachable from a third card on the Financial Calculators page.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

> **How it was published.** Rebuilt on calculator 1's shell rather than shipping the standalone
> preview: header, mobile menu and footer are byte-identical to the other two calculator pages, the
> shared stylesheet is linked instead of inlined, and the no-JS fallback comes with it. The 90KB
> preview became a 35KB page.
>
> **Checked on the live page**, desktop and 375px: $12,000 fixed with a $160 margin gives exactly 75
> sales and $4,000 profit at 100 sales; the default case still gives 84 sales and $2,200. No sideways
> scroll, nothing overflowing, the table scrolls inside its own box, tap targets 44px, no console
> errors. `/calculator-10-break-even.html` correctly returns nothing.
>
> **⏳ Question J stays open** — whether he wants "how long until I break even" as well. It was not
> built and must not be added without his answer.

**Added:** 2026-09-11 · *asked for by Shimon* · **Numbered 10** — see the
[calculator numbering](#calculators--the-permanent-numbering) section

A calculator that tells a small business owner how much they need to sell before the business covers
what it costs to run.

**Built for review 2026-09-11** at `C:\Users\Admin\Documents\outputs\break-even-calculator.html`.
Not on the site, not deployed.

**Four inputs:** fixed costs a month, price of one sale, what that sale costs, and optionally the
sales they make in a month. **The output:** how many sales a month covers everything, what that is in
revenue, a chart of the two lines crossing, a table of profit at different levels, and what they
would make at their own level of sales.

**Why it matters:** it is the first calculator that is about running a business rather than a
personal number, and it is the question most new clients arrive with.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon's request
> 2026-09-11.*
>
> **The arithmetic is trivial; the honesty is not.** Break even sales = fixed costs divided by the
> margin on one sale, rounded **up** to a whole sale. Everything else follows. Verified against a
> separate model on 58 cases with no mismatches, including the case where the division lands on an
> exact whole number and must not round up a further sale.
>
> **⚠️ Three decisions taken, all reversible, all his to overturn:**
> 1. **Per sale, not percentage margin.** He asked for price and cost per sale, and that is what most
>    owners can answer. The margin percentage is shown as a read back underneath instead, so an owner
>    who thinks in margin still sees their number. A business with hundreds of different prices should
>    use an average, which the tooltip says.
> 2. **Fixed costs are monthly**, and every figure on the page is monthly. Rent, wages and insurance
>    are what owners picture, and they picture them per month.
> 3. **"How long until I break even" was left out.** It is a different question and needs a startup
>    investment figure the calculator does not ask for. What is there instead is profit at the level
>    of sales they actually make, which answers the same worry without guessing. **See the open
>    question below.**
>
> **The degenerate cases are handled out loud, not hidden.** If the cost per sale is the same as or
> higher than the price there is no break even at any volume, and the headline says **"Never"** rather
> than printing a nonsense number. Where each sale loses money it says so and adds that selling more
> makes it worse. Roughly half of random inputs land in this territory, so it is not an edge case.
>
> **A bug worth remembering:** with zero fixed costs the break even is zero sales, and
> `Math.ceil` of a tiny negative returns **negative zero**, which prints as "-0 sales". It is clamped
> now. Any future calculator doing `Math.ceil` on a division should clamp the same way.
>
> **Nothing in the chart is focusable.** No `tabindex`, no click handler, pointer and touch only,
> following the rule set on calculator 1 after the black box.

---

## CALCULATORS — the permanent numbering

**Added 2026-08-27, at Shimon's instruction.** He wants to refer to these by number — "calculator 3"
— rather than by name.

### 🔒 THE NUMBERS ARE PERMANENT

**Never reuse a number. Never reorder them. Never renumber to close a gap.** If one is dropped, its
number is retired and stays retired. New calculators take the next free number. This is the whole
point of the scheme: a number he says out loud in six months must still mean the same thing.

### 🔒 THE NUMBERS ARE INTERNAL. THEY NEVER APPEAR ON A PAGE.

**Added 2026-08-27, at Shimon's instruction.** The numbering is shorthand between him and whoever is
doing the work. **A visitor must never see it.**

- **Not in the heading.** The page is headed with its plain name: "Compound Interest Calculator",
  "Mortgage Payment Calculator".
- **Not in the browser tab title.** Same plain name.
- **Not as an eyebrow, badge, breadcrumb, label or note anywhere on screen.**

**🔒 NOT IN THE WEB ADDRESS EITHER. Settled by Shimon 2026-09-03.** A URL is something a visitor sees,
types and pastes, so a number in it breaks this rule like any other. **Calculator pages are named for
what they are:** `compound-interest-calculator.html`, `retirement-calculator.html`. **Never
`calculator-1-...`.**

**Where the numbers do belong, and stay:** this registry, and conversation. That is all — **not the
file name.** The working drafts in `outputs\` still carry numbers in their names, which is fine: they
are never served to anyone. **The moment a calculator goes on the website it is renamed** to its plain
name.

**This binds calculators 3 and 8 when they are built**, and anything numbered after them. Build the
page with its plain public name from the start rather than adding a number and stripping it later.

| # | Name shown to visitors | Status | Published file name (no number) |
|---|---|---|---|
| **1** | Compound Interest Calculator | **🟢 LIVE — shipped 2026-09-02** (`626d9ab`→`66d8bac`) | `compound-interest-calculator.html` |
| **2** | Mortgage Payment Calculator | **🟢 LIVE — shipped 2026-09-03** (`76d83eb`) | `mortgage-calculator.html` |
| **3** | S-corp vs LLC savings | Wanted, not started | `s-corp-vs-llc-calculator.html` *(when it ships)* |
| ~~**4**~~ | ~~Quarterly estimated tax payments~~ | **DECLINED 2026-08-27** | — |
| ~~**5**~~ | ~~True cost of an employee~~ | **DECLINED 2026-08-27** | — |
| ~~**6**~~ | ~~Section 179 equipment purchase saving~~ | **DECLINED 2026-08-27** | — |
| ~~**7**~~ | ~~1099 contractor vs W-2 employee cost~~ | **DECLINED 2026-08-27** | — |
| **8** | Late filing and payment penalties plus interest | Wanted, not started | `penalties-and-interest-calculator.html` *(when it ships)* |
| **9** | Retirement Calculator | Wanted 2026-09-02, details not settled — see item 23 | `retirement-calculator.html` *(when it ships)* |
| **10** | Break Even Calculator | **🟢 LIVE — shipped 2026-09-11** (`213dfbb`) | `break-even-calculator.html` |

**Next free number: 11.** Numbers 4 to 7 are **retired, not free** — see below.

**Where things actually are, as of 2026-09-03:**

- **On the website:** the landing page `calculators.html`, and calculator 1 at
  `compound-interest-calculator.html`. Both live and reachable from the Resources menu.
- **Still working drafts in `C:\Users\Admin\Documents\outputs\`, not on the website:** calculator 2
  (`calculator-2-mortgage.html`), plus the earlier drafts of calculator 1 and the landing page and nav
  previews. **These keep their numbered names — they are never served to anyone.**

> **📎 The three "when it ships" names above are suggestions, not decisions.** They follow the
> convention Shimon settled on 2026-09-03 — plain name, no number, `-calculator` suffix, matching the
> one page actually live. **The names themselves are still his to approve** when each one ships; what
> is settled is that **no number appears in the address.**
>
> **Two corrections made here on 2026-09-03, both at his instruction ("yes to all"):**
> 1. The table said **"None of them is on the website."** Calculator 1 has been live since 2026-09-02.
>    Corrected above.
> 2. The File column carried numbered names like `calculator-1-compound-interest.html`, which is not
>    what shipped and would have put a number in a public web address. Corrected to the published
>    names, and the rule is now stated in the "numbers are internal" section above.

### A menu item to reach them

**✅ SETTLED AND SHIPPED 2026-09-02 — but not the way this section proposed. Read the next paragraph
before acting on anything below it.**

What shipped is **"Financial Calculators" as a third entry inside the existing Resources dropdown** —
not a new top-level heading between Resources and About, and not the recommended shorter name. So the
naming question below is closed, and the width measurements below no longer describe the live bar:
nothing was added to the top level, so the crowding problem the measurements were about **did not
arise.** Verified live 2026-09-02: the entry appears exactly once in the desktop dropdown and once in
the phone menu, on all 15 pages, and there is no sideways scroll at 375px.
*Everything below is left in place as the record of what was considered and measured.*

**Added 2026-08-27.** In his words: *"add on the website a new header called financial calculators or
give me a better name that fits in well with a drop down and for now let's put the compound interest
one make me a html"*.

**Preview built, not on the site:**
`C:\Users\Admin\Documents\outputs\hirsch-nav-preview.html` (open this one)
with `hirsch-nav-frame.html` beside it, which it loads twice to show a computer and a phone.

**The name is his to settle.** Three were offered: **Calculators** (recommended), **Tools**, and his
original **Financial Calculators**. It is a one word change whichever he picks.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon's request,
> 2026-08-27.*
>
> **Why Calculators was recommended, with the measurement behind it.** Every other item in his bar is
> a single word: Services, Resources, About, Contact. "Financial Calculators" is two words and 21
> characters against About's 5. Measured in a browser at 1000, 1200 and 1440 pixels: with
> **"Financial Calculators" the gap between the logo and the menu is 0px at every one of those
> widths**, so the bar is pressed tight against the two buttons on the right. With "Calculators" the
> gap is 65px at 1200 and 1440, and with "Tools" it is 105px. **All three are tight at 1000px**,
> which is worth knowing: the bar is already close to full today, before anything is added.
>
> **Where it sits and how it behaves.** Between Resources and About. On a computer it opens on
> pointing, like the two dropdowns already there. On a phone there is no hover, so it becomes another
> expanding heading in the slide down menu, exactly like Services and Resources. Verified at 375px:
> the desktop bar is hidden, the heading is a 49px tap target, the list opens and closes, and there
> is no sideways scroll.
>
> **Built so the rest drop in.** Each calculator is one line in the computer dropdown and one line in
> the phone menu. **Both spots carry the comment `CALCULATORS: one line each`** so nobody has to hunt
> for them. Calculators 2, 3 and 8 are two lines each when approved.
>
> **A quirk carried over deliberately.** Clicking the word "Calculators" itself goes to the first
> calculator rather than doing nothing, because that is what "Resources" already does on the live
> site. It was flagged in the design audit as odd, but matching the existing behaviour beats
> introducing a third pattern. **Change both together or neither.**

---

### DECLINED — do not propose these again

Shimon was offered six tax calculators on **2026-08-27** and cut it to two the same day. In his
words, of the four below: **"for sure not."**

- ~~**Calculator 4** — Quarterly estimated tax payments~~
- ~~**Calculator 5** — True cost of an employee (wage plus payroll taxes)~~
- ~~**Calculator 6** — Section 179 equipment purchase saving~~
- ~~**Calculator 7** — 1099 contractor vs W-2 employee cost~~

**He kept 1, 2, 3 and 8.** That is the whole set.

**🔒 Their numbers are retired, not recycled.** Do **not** renumber calculator 8 down to 4 to close
the gap, and do **not** hand 4, 5, 6 or 7 to some future calculator. The gap in the sequence is
correct and intended. If he ever revives one of these four, it comes back **under its own original
number**, not a new one.

**These were Claude's suggestions in the first place, not his** — they came out of the comparison
with schapiracpa.com. He has now looked at the list and said no. Do not re-pitch them as fresh
ideas, and do not fold them in as "while we're building calculator 3 we could also…".

### The style brief — applies to every one of them

In Shimon's words: **"make the calculators simple and user friendly"** and **"not too complicated,
it's geared for regular people not accountants."**

That means, on every calculator:

- **As few inputs as possible.** If a normal person wouldn't know a figure, work it out for them,
  give it a sensible default, or leave it out — don't ask.
- **Plain English labels.** "Money you're putting down", not "Down payment (principal reduction)".
  No tax jargon on the face of the page.
- **One clear headline answer**, not a table. A single big number and one plain sentence under it.
- **Detail behind a "Show the breakdown" toggle**, closed by default.
- **Sensible defaults**, so it shows a real answer before anyone types anything.
- **No dashes in anything a visitor reads.** Standing preference, stated 2026-08-27. Use a full stop,
  a comma or a rewrite instead. Hyphens inside a phone number are fine.
- **Thousands separators on every number he sees**, including inside the input fields as he types.
  `1,000,000`, never `1000000`. Added 2026-08-27 at his instruction.

> **📎 How the comma formatting is built, so it is copied rather than reinvented.** A browser's
> `type="number"` field **refuses to hold a comma**, so every money field is `type="text"` with
> `inputmode="decimal"` (which still brings up the numeric keypad on a phone). A small `fmtField`
> helper reformats on every keystroke and on blur, and **puts the caret back by counting digits
> rather than characters**, otherwise it jumps to the end mid-typing. `num()` strips commas before
> parsing. Both are already written in calculators 1 and 2 and should be lifted from there.
> **Rate and year fields stay plain number inputs** because they never reach four figures and a
> comma rule would fight decimal entry on the rate. Tested: typing, pasting a formatted value,
> pasting junk, decimals, inserting mid number, and backspacing over a comma.

**This brief overrides any reference site.** Calculator 1 was originally modelled closely on
moneygeek.com and was deliberately simplified afterwards when he gave this instruction — the
reference lost, the brief won. Do the same for any future reference.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon's instruction,
> 2026-08-27.*
>
> **What "simplified" actually meant in practice**, so the level is reproducible rather than guessed:
>
> - **Calculator 1** went from 5 controls to 4. The Monthly/Annually contribution toggle was dropped
>   (monthly is what people do), the chart went from three stacked colours to two ("money you put in"
>   vs "interest earned"), and the four-row breakdown moved behind a toggle. The headline gained a
>   plain sentence: *"You'd put in $23,000 of your own money and earn $6,542 in interest on top."*
> - **Calculator 2** went from 8 controls to 4. The dual dollar/percent deposit boxes became one
>   dollar box with a live "That's 20% of the price" line underneath. Property tax, insurance and HOA
>   moved into the breakdown as **optional** fields that start empty. The headline is now the loan
>   repayment alone, with a visible note that tax and insurance come on top — because guessing a
>   property tax rate for a stranger is exactly the silent assumption that should be avoided.
> - **Mortgage insurance was removed entirely** from calculator 2. The earlier version added it
>   automatically below 20% down using an assumed 0.5%/year. That assumption was never approved, and
>   it is jargon a regular person doesn't need — it is now named in the disclaimer as something
>   lenders add, rather than silently priced in.
>
> **The maths did not change when they were simplified.** Calculator 1 still reproduces the
> reference's own default result exactly ($5,000 + $150/month at 4% for 10 years = **$29,542**), and
> calculator 2's amortisation still agrees with the independent formula to the cent
> (**$2,275/month** on $360,000 at 6.5% over 30 years). Both were re-tested after simplification
> against zero rates, zero contributions, a 100% deposit and junk input.
>
> **Both disclaimers were rewritten in plainer English at the same time.** The wording is in items 16
> and 17. **Still unapproved — do not publish either without his sign-off** (Rule 7).

---

## OPEN QUESTIONS — only Shimon can answer these

These are **not defects.** They are three statements the site makes that no amount of checking from
the outside can confirm or disprove. They are here because the site's standing rule is that nothing
published may be untrue, and each of these is either true or it is a problem — and only Shimon knows
which.

### A. ✅ ANSWERED — Does info@hirsch.cpa actually reach a mailbox somebody reads?

**Asked:** 2026-08-26 · **Answered by Shimon 2026-08-27: YES.** The address reaches a monitored
mailbox. **Closed — do not raise again.**

**What this settles:** email is a working way to reach the firm, so while the contact form is dead
(item 2) visitors are not left with only the telephone. It does **not** reduce the urgency of item 2
— someone who uses the form still believes they made contact and still gets nothing. It also answers
half of item 2's open decision: `info@hirsch.cpa` is a live monitored mailbox and is therefore a
candidate for where form messages should go, though **he still has to confirm that is the address he
wants them sent to.**

That address appears thirty times across the site and is currently the only working way to contact the
firm, since the form does nothing (item 2). The firm's mail is set up and running — but whether this
particular address exists and is watched by a person cannot be checked without emailing it, which the
audit deliberately did not do.

**If the answer is no,** then the site currently has **no working way at all** for a prospective client
to make contact except the telephone, and item 2 goes from serious to urgent.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26.*
>
> **What is known.** `info@hirsch.cpa` appears 30 times across the 12 pages, always as a `mailto:`
> link, in the footer of every page plus the contact panels and the Contact-us paragraphs of the
> privacy and terms pages. The domain's MX record points to
> `hirsch-cpa.mail.protection.outlook.com`, so firm mail is hosted on Microsoft 365 and the domain
> can receive mail. **Whether this specific mailbox or alias exists, and whether anyone reads it, is
> unknown.**
>
> **Why it wasn't tested.** Sending a test email is a write to a live system and would put a real
> message in front of a real person. The audit rules are read-only, GETs only, zero writes — so it
> was deliberately not done. **Do not "just send a test" to close this out; ask Shimon.**
>
> **Other firm addresses that exist in the wider practice** (from the practice-manager docs, not from
> this site): `shimon@hirsch.cpa`, `Joseph@hirsch.cpa`, and `office@hirsch.cpa` as a Brevo sender.
> None of these appears on the website. If `info@` turns out not to exist, one of these is presumably
> the intended destination — but that is also the open decision in item 2 ("which address"), so
> **answer both together.**

---

### B. ✅ ANSWERED — Are the AICPA and NYSSCPA memberships shown on the home page current?

**Asked:** 2026-08-26 · **Answered by Shimon 2026-08-27: YES.** Both memberships are current.
**Closed — do not raise again.**

**What this settles:** the seals and the "Members of the AICPA & NYSSCPA" wording are true as
published, so nothing has to be removed or softened. It also unblocks **I4** (making the affiliations
row more prominent) and **M18** (a glow behind the CPA seal) — both were held back because drawing
attention to an unverified claim would have made it worse. They are now safe to build on their own
merits.

The home page displays both organisations' logos as membership seals, and the wording "Members of the
AICPA & NYSSCPA" appears on several pages.

**If either has lapsed,** it is a claim about professional standing on the public site of a regulated
practice, which is exactly the category of statement that has to be right.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26.*
>
> **Exactly what is claimed, and where:**
> - `index.html` trust band — three seals: a "CPA / Licensed / Certified Public Accountants" badge;
>   `assets/aicpa.png` (alt "AICPA") captioned **"Member of — American Institute of CPAs"**;
>   `assets/nysscpa.png` (alt "NYSSCPA") captioned **"Member of — New York State Society of CPAs"**.
> - `index.html` hero `.microtrust` — "**Licensed CPAs** · Members of the AICPA & NYSSCPA".
> - `index.html` About section `.creds` — "Licensed Certified Public Accountants based in New York ·
>   Members of the AICPA & NYSSCPA".
>
> So it is claimed three times on the home page, twice in words and once with both organisations'
> logos reproduced.
>
> **Two things are being asserted, not one:** current membership of both bodies, **and** an implied
> licence to use their marks. Some professional bodies restrict logo use to members in good standing.
>
> **This is unverifiable from outside** — there is no public membership register to check against —
> which is why it is a question and not a finding. It falls squarely under Rule 7 in `CLAUDE.md`
> (never publish a statement that isn't true), and Rule 7 is the reason to raise it rather than let
> it sit.

---

### C. Two pages tell prospective clients their completed returns are waiting in the portal

**Asked:** 2026-08-26

The Tax Preparation page says *"your completed return is available anytime through the client
portal,"* and the home page says *"Access your returns anytime through our secure client portal."*
The portal exists and its login page works.

Shimon has said the portal does not currently hold anything. If that is still so, both sentences
describe something a new client would expect on day one and would not find. The choice is his: either
the portal gets stocked, or the two sentences get softened to describe what it will do rather than
what it already does.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: design audit (Audit B),
> 2026-08-26.*
>
> **The three statements, verbatim:**
> - `index.html`, "Secure portal" column — *"Access your returns anytime through our secure client
>   portal."*
> - `services/tax-preparation.html`, "How it works" — *"Once filed, your completed return is
>   available anytime through the client portal."*
> - `privacy.html`, "Client confidentiality" — *"Documents made available through our secure client
>   portal are protected by access controls and encryption."* (A weaker claim: conditional on
>   documents being there. Included so it isn't missed when the other two are edited.)
>
> **What was verified.** `https://hirsch-portal.vercel.app` returns 200 and redirects to `/login`.
> The Client Login button in the header, the mobile menu and the footer of all twelve pages points
> there, `target="_blank" rel="noopener"`. So the portal is real and reachable. **Whether it holds any
> client documents was not and cannot be checked from the website** — that would need signing in,
> which is out of bounds.
>
> **Note the overlap with item 1:** the portal is on a temporary vercel.app address too, so if
> Shimon's answer is "stock it", the domain work in item 1 should cover the portal in the same pass.
>
> **The lighter fix, if he wants one:** the home page and service page sentences are present tense
> ("available anytime"). Softening to what a client gets once the firm has filed for them would make
> both true immediately without any portal work. Offer it as an option; **do not rewrite copy about
> the firm's services unasked** (Rule 3).

---

### D. ⚠️ PARTLY ANSWERED — Should the motion feel restrained, or lively?

**Asked:** 2026-08-27 · **Shimon's answer 2026-08-27: "could be better."** **Still open — this is a
direction, not a setting.**

Read his answer as: **the site as it stands feels too plain to him, and he wants more life than it
has now.** That rules out "leave it restrained as it is." It does **not** say how far to go, which is
the part still needed.

**Until he pins it down,** keep building toward the restrained-but-livelier end — noticeably more
alive than today, well short of the comparison site. It is easier to add energy later than to take it
back off a professional firm's site.

**Ask him again before the bigger motion work** — specifically before M3 (which fixes one speed and
easing for the whole site) and before anything in AMBIENT.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Why it is worth settling early.** This single answer sets the duration and easing tokens in M3,
> the travel distance in M6, and how much of the AMBIENT group (M16–M19) gets built at all. Answering
> it after those are built means redoing them.
>
> **What each answer means concretely.** *Restrained*: ~0.35–0.45s, 12–14px travel, gentle easing,
> AMBIENT limited to the rotating badge alone. *Lively*: faster and larger movements, more of AMBIENT,
> possibly the marquee in M19.
>
> **The reference point.** The comparison site is firmly at the lively end — 22 animations running at
> once, three infinite loops, a 3D object. **Do not assume that is what he wants** just because he
> admired the site; he may be responding to its substance (see the note under IDEAS) rather than its
> energy. **Ask, do not infer.**

---

### E. Which figures about the firm is he willing to publish?

**Asked:** 2026-08-27

The counting-numbers effect he liked needs numbers to count. The site currently states no figures
about the firm at all — no years in practice, no client count, no returns filed.

**Nothing in the NUMBERS group can be built until he supplies these**, and every figure has to be one
he can stand behind.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Blocks M9, M10 and M11 completely.** M10 is the item that supplies the content; M9 animates it;
> M11 makes it safe without scripts. None can start without an answer here.
>
> **⚠️ Do not source these numbers yourself.** A client count is derivable from the practice-manager
> app's database, and using it would be publishing a real figure about a regulated practice that
> Shimon never approved. **Rule 7 — ask him for the numbers, do not calculate them.** He is also the
> only one who knows which are commercially sensible to publish.
>
> **Why this question matters more than the rest of the motion work.** M10 is the only item in the
> MOTION section that also closes part of the credibility gap identified in IDEAS — it is
> simultaneously the animation he asked for and the evidence the site lacks. **If he engages with one
> question in this group, steer him to this one.**

---

### F. What should the rotating badge say?

**Asked:** 2026-08-27

He liked the slowly turning circle on the other firm's site and wants one. What text runs around it
is his call — the firm's name, a founding year, or the credentials.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Blocks M16.** The mechanism is trivial — text on a circular SVG path with a slow CSS rotation —
> so the wording is the entire decision. **A rotating ring saying something vacuous is worse than no
> ring**, because it draws the eye to filler.
>
> **Options, none chosen:** the firm name ("HIRSCH & CO. ACCOUNTING LLC ·"), a founding year
> ("EST. ——"), or the credentials ("CERTIFIED PUBLIC ACCOUNTANTS ·").
>
> **⚠️ If he picks a founding year, Claude does not know it — ask.** Do not infer a year from the
> domain registration, the git history, or anything in the practice-manager app. A wrong founding
> year on a regulated firm's public site is a Rule 7 problem.

---

### G. Does the motion work happen before or after the contact form and domain?

**Asked:** 2026-08-27

Items 1 and 2 — the domain showing a security warning, and the contact form losing enquiries — are
the two things on this list that are actively costing the firm. The motion work is polish. He has
approved four motion changes to be built now, so in practice he has answered "alongside," but the
larger question of sequencing is still open.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **This is a judgement call that is genuinely his, and he has partly made it** — on 2026-08-27 he
> approved M5, M6, M7 and M8 for immediate build. Do not re-litigate that.
>
> **The honest position to hold if he asks.** The motion work is cheap, low-risk and entirely within
> his control; the domain and form both need decisions and outside services. There is no technical
> reason they compete. The only real cost of doing motion first is that the site gets livelier while
> still losing enquiries — **which is worth saying once, plainly, and then dropping.** He has been
> told; it is his firm.
>
> **One genuine dependency worth flagging:** M24 and I24 both add or restyle routes to the Contact
> page. Making those routes more prominent while the form is dead in item 2 makes that problem
> *bigger*, not smaller. Sequence those two behind item 2 specifically, regardless of the general
> answer here.

---

### H. ✅ ANSWERED — On the mortgage calculator, should the big figure be the loan repayment or the full monthly cost?

**Answered 2026-09-03: the FULL MONTHLY COST**, including property tax and home insurance. Built into
the draft the same day; awaiting his review of the draft, not deployed.

> **📌 How the risk he was warned about is handled — read this before changing any of it.** The danger
> was that tax and insurance are optional and start empty, so a headline labelled "full monthly cost"
> would silently understate the real cost for anyone who left them blank. **The figure and the words
> now always agree:**
> - **Both boxes empty:** the line reads *"Your monthly payment would be"*, the figure is the loan
>   repayment alone, and the note says in bold that tax and insurance are not in it and where to add
>   them.
> - **Either box filled:** the line becomes *"Your full monthly cost would be"*, the figure includes
>   whatever was entered, and the note lists exactly what is in it — **and names in bold anything
>   still missing.** Fill in tax but not insurance and it says so outright.
> - A zero or blank counts as not entered, so a stray `0` cannot be mistaken for a real figure.
>
> The loan repayment on its own did not disappear: it is a row in the breakdown view, labelled
> *"Loan repayment on its own"*.
>
> **Never let the headline claim a component that was not entered.** That is the whole point of this
> answer, and it is easy to undo by "simplifying" the label logic.

**Asked 2026-09-03 · originally flagged to him with the draft.**

As the draft stands, the one large figure is **the loan repayment only** — principal and interest.
Property tax and home insurance are added on top and appear in the breakdown view, as "Full monthly
cost". MoneyGeek does the opposite: its headline is the **full monthly cost**, with principal and
interest shown underneath as a component.

**Both are defensible and it is genuinely his call:**

- **Loan repayment as the headline** *(what the draft does)* is the number a lender quotes and the
  number he would say out loud to a client. It is also the only part the calculator can know exactly.
- **Full monthly cost as the headline** is the number that actually leaves someone's bank account, so
  it is the more honest answer to "what will this cost me" — but it is only right if they filled in
  the tax and insurance boxes, which are optional and start empty.

**The awkward case that decides it:** if the headline is the full cost and someone leaves tax and
insurance blank, the big number silently understates what they will really pay. The draft's current
arrangement avoids that by never claiming to be the full picture.

> **📎 CONTEXT FOR CLAUDE.** Do not change this on your own initiative — it was a deliberate choice,
> not an oversight. If he picks the full cost, the empty-boxes case must be handled on the page, not
> left to be discovered. Related: item 27, where "headline figure is the full monthly cost" sits in
> the MoneyGeek list.

### I. ✅ ANSWERED — Does he approve the line under the heading on the mortgage calculator?

**Answered 2026-09-03: yes, he accepted the wording as drafted.** He did not supply his own text, and
none is needed. **The sentence is settled and stays as it is.**

> **📌 Note the difference from calculator 1, so nobody draws the wrong lesson.** On the compound
> interest calculator ([item 24](#24-change-the-description-on-the-compound-interest-calculator)) he
> wrote the line himself and it was used character for character. Here he read a drafted line and
> approved it. **Both routes are legitimate — the rule is that he decides, not that he must always
> write it.** Do not "improve" this sentence later on the grounds that it was not his; he has read it
> and accepted it.
>
> **Still to remember when this page ships:** the equivalent description text also lives in the
> `meta`/`og`/`twitter` tags and on the `calculators.html` card. Item 24's block records that trap.

**The sentence, as approved.** *"Estimate what a home
loan would cost you each month. Enter the price, what you are putting down, the interest rate and how
long you would pay it over to see your payment and what the loan costs in total."*

It was written to match the shape of the wording **he supplied** for the compound interest calculator
on 2026-09-03, because the draft still carried the old "Fill in your figures, then press Calculate."
line that he had already replaced on calculator 1.

**It needs his text or his approval before the page goes live.** He supplied his own words last time
rather than accepting a draft, so the likelihood is he will want to here too.

> **📎 CONTEXT FOR CLAUDE.** This is the same job [item 24](#24-change-the-description-on-the-compound-interest-calculator)
> did for calculator 1 — that one is closed because **he** supplied the text. **Do not close this one
> by writing a better sentence.** Only his wording, or his explicit approval of this one, closes it.
> If it is his wording that lands, remember the equivalent text also exists in the meta/og/twitter
> description tags and on the `calculators.html` card — item 24's block records that trap.

---

### J. On the break even calculator, does he want "how long until I break even" as well?

**Asked 2026-09-11 · ⏳ FLAGGED TO HIM, NOT YET ANSWERED.**

The calculator answers **how much** they need to sell. It does not answer **how long** it will take,
which is often the real worry underneath the question.

**It was left out deliberately, because "how long" means two different things** and the calculator
cannot tell which one is meant:

- **"When do my monthly sales cover my monthly costs?"** That is a level of sales, not a length of
  time, and the calculator already answers it.
- **"When do I get back the money I put in to start?"** That is a genuinely different sum. It needs
  a startup investment figure the calculator does not ask for, plus a view on how sales grow month by
  month, which is the shakiest guess in the whole exercise.

**What is there instead:** if they type in the sales they actually make, it shows what that leaves
them after everything. That answers the worry without inventing a growth curve.

> **📎 CONTEXT FOR CLAUDE.** If he wants the second version, it is one more input (money put in to
> start) and one more output, but **it also needs a stated assumption about sales growth, and that
> assumption is doing most of the work in the answer.** Say so on the page if it is built. Do not
> quietly assume flat sales; a new business with flat sales from day one is not the normal case.

---

## REFERENCES — sites Shimon wants ideas taken from

Not defects and not work in themselves. These are sites he has pointed at as a source of ideas for
how this one could look or work. **Nothing here is a decision.** He has not said which parts he
likes, and no Claude should assume — ask him what he wants taken from one before building anything.

### R1. Schapira CPA — another CPA firm's site, for ideas

**Added:** 2026-08-27

**The link:** <https://www.schapiracpa.com/>

Shimon wants this kept on the list as a reference to take ideas from for the firm's website. He has
not said which parts of it he has in mind.

**Neutral notes on what it does**, from looking at it on 2026-08-27 — observations only, offered as
context for when he says what he wants:

- Another Brooklyn CPA firm, but aimed at one industry only: manufacturers. Its home page leads with
  that focus rather than with a general list of services.
- It sets out five named services, the industries it works with, client case studies with figures
  attached, testimonials, and a blog. It also offers calculators.
- **It has real online booking.** Its "Book Your Call" button leads to a page with a booking calendar
  built into it, offering a 30-minute discovery call that a visitor picks a slot for and confirms
  there and then. (Item 4 on this list is the open question of which calendar service to use here;
  this is one working example of what that looks like, not a recommendation to copy it.)
- **Client Login** goes out to a third-party client portal rather than one the firm built itself.
- There is no contact form on its home page — the routes offered are the booking page, a phone
  number and an email address.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: Shimon's request,
> 2026-08-27; observations from a read-only look at the live site the same day.*
>
> **Shimon has said only that he wants ideas taken from it.** He has NOT said which parts he likes.
> Do not infer preferences from the notes below and do not propose a redesign off the back of them.
> The correct next move is to ask him what he wants taken from it.
>
> **Technical observations (2026-08-27):**
> - Title: "Schapira CPA | Manufacturing CPA Firm | Brooklyn, NY". Positioning is vertical-specific —
>   manufacturers only — with heavy trademark-style branding ("ProFit™", "the Profit Method").
> - Booking: `/consultation` embeds **Calendly** inline
>   (`calendly.com/shragy-schapiracpa/30min-discovery`, via `assets.calendly.com/…/widget.js`),
>   headed "Book Your 30-Minute Discovery Call". Both "Book Your Call" and "Book Your Strategy Call"
>   CTAs route there. This is the concrete mechanism behind item 4's open question.
> - Client Login → `onvio.us/clientcenter/…` — Thomson Reuters Onvio, an off-the-shelf portal, not
>   self-built. Contrast with hirsch.cpa's own portal, which is custom.
> - **Zero `<form>` elements** on both the home page and the consultation page. Contact routes are
>   the booking embed, a phone number and an email address only.
> - Content types present that hirsch.cpa does not have: case studies with dollar figures and
>   percentage profit increases, named testimonials with company attributions, a blog / "Latest
>   Insights", and calculators.
> - It runs a Facebook pixel (`connect.facebook.net/en_US/fbevents.js`). Worth noting only because
>   hirsch.cpa currently runs **no** tracking at all, and item 3 records that as a fact about the
>   privacy policy — adding tracking would change what that policy has to say.

---

## IDEAS — from the comparison with schapiracpa.com

**Added 2026-08-27.** Shimon said the other firm's site (item R1) looks far more professional than
his and asked what to change. Both sites were compared on desktop and phone. He then went through
the resulting list himself and kept these — **they are his decisions, not proposals awaiting
approval.** Three ideas he explicitly rejected are recorded at the end of this section so nobody
raises them again.

**These are ideas, not defects.** Nothing here is broken. They are changes that would make the site
read as more established. They are numbered **I1–I27** so they never collide with the numbered
problems in OPEN. **Groups are his groupings** — keep them, he uses them to scan.

**Standing rule applies to every one of these:** they change how the site looks, so under Rule 2 in
`CLAUDE.md` each one gets an HTML preview shown to him **before** it is built. None of these is
approved to build — he has approved them onto the list.

### PROOF

#### I1. Add case studies with actual numbers: what the client faced, what changed.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **What the other site does.** Three case studies on its home page, each with a financial baseline
> and a profit increase stated as a figure — "$1,200,000 / 23.4%", "$10,000,000 / 18.0%",
> "$220,000 / 15.0%" — with headlines like "$30M in Sales, Losing Money: The Inventory Fix". They
> link through to a case-studies section.
>
> **Why it carries the weight.** This is the single largest gap between the two sites. Everything on
> hirsch.cpa describes *categories of service*; this describes *work actually done*. Specific
> numbers are what a reader treats as evidence rather than claim.
>
> **What implementing it involves.** New content Shimon has to supply — Claude cannot invent client
> outcomes. Needs a page or home-page section, plus a decision on anonymising ("a Brooklyn
> distributor" rather than the client's name). **Client confidentiality applies: no client is named
> or made identifiable without written permission.** Any figure published must be one he can stand
> behind.

#### I2. Add client testimonials with the person's name and their company.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **What the other site does.** Named quotes attributed to a person and their firm — e.g. a CEO of a
> named company. Attribution is what separates a testimonial from marketing copy; an unattributed
> quote reads as invented.
>
> **What implementing it involves.** Shimon has to gather them and get permission to publish name and
> company. Needs a section on the home page or a dedicated page. **Do not write, paraphrase or
> "tidy" a client's words** — publish what they said or don't publish it.

#### I3. Put a concrete result on each service page, not just a description.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **What the other site does.** Its tax-planning page carries a specific outcome line —
> "12% tax reduction for a medical equipment client" — sitting inside an otherwise descriptive page.
> One sentence of evidence per page.
>
> **Current state here.** All six service pages are description-only: "What it covers", "Who it's
> for", "How it works". No outcome, figure or example anywhere.
>
> **What implementing it involves.** Six short factual lines Shimon supplies, one per service page,
> in the existing page furniture. Same confidentiality constraint as I1. Smaller job than I1 and a
> reasonable place to start.

#### I4. Add the professional bodies you belong to as a proper affiliations row.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **⚠️ The site already has one — check before proposing anything.** `index.html` has a `.trust`
> band directly under the hero with three seals: a "CPA / Licensed" badge, AICPA captioned "Member of
> — American Institute of CPAs", and NYSSCPA captioned "Member of — New York State Society of CPAs".
> This idea is an *improvement to something that exists*, not a new thing to build.
>
> **The three real differences from the other site.** (a) It lists **three** bodies (AICPA, NYSSCPA,
> **PICPA**) — Shimon may belong to bodies or hold licences not currently shown; that is a question
> for him, not something to research. (b) Its affiliations sit in a dedicated, labelled block on its
> About page as well as elsewhere — his appear once, on the home page only. (c) His logos render
> small — AICPA at 54×54px, NYSSCPA at 64×41px — and the caption text beside them is the
> low-contrast grey flagged in item 6.
>
> **What implementing it involves.** Ask him which bodies and licences he actually holds; enlarge the
> marks; fix the caption contrast alongside item 6; consider repeating the row where credibility is
> being judged. **Cross-check Question B first** — whether those memberships are current is still
> unanswered, and enlarging an unverified claim makes it worse, not better.

### FOCUS

#### I5. Lead with who you're for, not what you do.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **What the other site does.** Opens with "The manufacturer's firm." — audience first, service
> second. Current hirsch.cpa hero opens with "Accounting and tax, handled with precision and care."
> — service and manner, no audience.
>
> **⚠️ Constraint he has set.** He rejected niching by industry ("we serve everyone"). So "who
> you're for" must be framed by *situation or need* — business owners who want their personal and
> business filings handled together, firms filing across multiple states, and so on — **not by
> sector.** See the rejected list at the end of this section.
>
> **What implementing it involves.** A rewritten hero headline and sub-line. Copy only; his words,
> his call.

#### I6. Make the headline about what the client gets, not how the firm works.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **The contrast.** Other site: "Grow a business others want to buy." — an outcome for the reader.
> His: "Accounting and tax, handled with precision and care." — a description of how the firm
> behaves. One promises the reader something; the other describes the supplier.
>
> **What implementing it involves.** Copy only, and it overlaps with I5 — treat them as one editing
> pass on the hero rather than two changes. He supplies the promise; do not invent one for a
> regulated practice.

#### I7. Say what makes the firm different in one line a competitor couldn't copy.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **⚠️ READ THIS BEFORE PROPOSING ANYTHING.** The obvious answer is industry specialisation — that is
> how the comparison site does it, and **Shimon has explicitly rejected it.** His words: *"we serve
> everyone."* Any differentiator proposed here **must be something other than sector.**
>
> **Directions still open**, none chosen: responsiveness and reachability (already the site's "The
> firm you can actually reach" theme, currently asserted rather than evidenced); personal and
> business filings coordinated by one team; multi-state complexity; year-round contact rather than
> filing-season only; the client portal. **Ask him — do not pick one.**
>
> **Why it's hard.** The current claims ("Responsive", "Personal attention", "You're a client we know,
> not a case number") are all things any firm can and does say. The test is whether a competitor
> could put the same sentence on their site unchanged. Today, they could.

#### I8. Drop "full-service" and similar phrases every firm uses.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Where it appears.** `index.html` About section: "Hirsch CPA is a **full-service** accounting and
> tax firm serving businesses and individuals." Related generic phrasing on the same page:
> "Everything under one roof", "real accounting rigor with modern tools and genuinely personal
> service".
>
> **Why it costs.** These phrases carry no information — a reader has seen them on every accounting
> site and skips them. Space spent on them is space not spent on something only this firm can say.
>
> **What implementing it involves.** Small copy edit. Depends on I7 being answered first, or the
> replacement is just a different generic phrase.

### LOOK

#### I9. Set large headings in a lighter weight — the bold serif reads heavy.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27. Measured on both live sites.*
>
> **Measured difference.** Other site: headings at **weight 300** (light), 36–48px. His: **weight
> 600** Fraunces serif throughout — h1 39px/600 on mobile, section h2s 30–40px/600.
>
> **What is doing the work.** Large text at light weight reads as contemporary and confident; large
> text at semibold reads as insistent. This is probably the largest single contributor to the
> *visual* half of the gap, as distinct from the content half.
>
> **What implementing it involves.** Fraunces is already loaded at weights 500 and 600. Dropping
> display headings to 500, or loading a lighter weight, changes every page at once — so this is a
> whole-site look change and squarely a Rule 2 preview. **Do not apply it to body text**; only
> display headings.

#### I10. Make headings noticeably bigger, especially on the phone.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Measured.** At 375px the other site runs section headings at 36px and its case-studies heading at
> 48px. His run 30px for section headings, 39px for the h1. Its type scale is more dramatic —
> bigger jump between heading and body — which is what creates a sense of hierarchy.
>
> **What implementing it involves.** Adjusting heading sizes in the mobile breakpoint. Pairs
> naturally with I9 and I12 — bigger *and* lighter *and* with more space around it is one coherent
> change; doing only one of the three will look wrong.

#### I11. Add one dark, high-contrast section to break up the cream.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **What the other site does.** Runs largely black (`#000` and `#1a1a1a`) with gold accents. His runs
> cream throughout (`#FBF8F2` and `#F6F0E5`) with one dark band — the "Let's talk" panel over the
> skyline photo.
>
> **The judgement.** Not a recommendation to go dark; a firm's site being warm and light is a
> legitimate choice and arguably better suited to an accounting practice than a black site. The point
> is *rhythm* — his page alternates cream/white/cream with little tonal variation, so nothing stands
> out. He already has one dark band that works; a second, placed differently, would give the page
> structure.
>
> **What implementing it involves.** Choosing which section goes dark and reworking its colours.
> Squarely Rule 2 — preview it.

#### I12. Give each section far more vertical breathing room.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Measured.** The other site's home page is **12,987px** tall on mobile carrying ~3,000 words. His
> is **6,648px** carrying ~443 words. Theirs devotes far more vertical space per idea — individual
> service blocks run 700–900px tall each. His sections are 522–2,081px for the whole block.
>
> **What it signals.** Generous space reads as confidence; tight space reads as a brochure. Current
> section padding is 82px desktop / 56px mobile.
>
> **What implementing it involves.** Increasing section padding site-wide — every page, so a full
> preview. Note this makes the page longer, which only helps if there is content worth scrolling
> past; **pair it with the DEPTH items rather than doing it alone.**

#### I13. Use a darker gold — the current one is slightly hard to read on white.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **This is the same change as item 6 in OPEN** — do not do it twice. `--gold #9C7430` gives white
> text 4.24:1, under the 4.5:1 standard; `--gold-d #7C5A22` already in the palette gives 6.28:1 on
> white. Item 6 has the full measurement table.
>
> **The comparison angle.** The other site uses gold at higher contrast against black
> (`#C89543`, `#D4AF37`), which is why its gold reads as crisp rather than muddy. His gold is fighting
> a cream background.
>
> **What implementing it involves.** Change the button background token. One value, affects every
> page. **Close item 6 and this together.**

#### I14. Increase the small grey text under the logo and beside the seals.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Also overlaps item 6 in OPEN.** The "Certified Public Accountants" line under the logo is **9px**
> at 3.74:1; the seal captions use the same `--muted #8B7E6C`. Item 6 covers the contrast; this adds
> the size point.
>
> **What implementing it involves.** Raise the 9px line and darken `--muted`. Do it as one change
> with item 6 and I13 — all three are the same few tokens in `:root`.

### DEPTH

#### I15. Triple the length of each service page.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27. Word counts measured on both live sites.*
>
> **Measured.** His tax-preparation page: **199 words**, 4 headings, 1 image. The other site's
> tax-planning page: **816 words**, 13 headings, 6 images. Across the whole home page it is ~443
> words versus ~3,002.
>
> **Why it reads as more established.** Depth signals expertise; a 199-word service page reads as a
> placeholder regardless of how well it is designed. This is the content half of the gap and it is
> larger than the design half.
>
> **What implementing it involves.** Substantial writing across six pages, and the content must be
> accurate — this is a regulated practice describing services it provides. **Shimon supplies or
> approves every claim.** Pairs with I16.

#### I16. List the specific things you actually do — R&D credits, Section 179, multi-state nexus, cost segregation.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **What the other site does.** Its tax-planning page names concrete instruments: R&D tax credit
> optimisation, Section 179 and bonus depreciation, multi-state and nexus planning, entity structure
> planning, cost segregation studies. Specific technical nouns read as competence in a way that
> "tax planning and projections" does not.
>
> **⚠️ The examples above are the OTHER FIRM'S list, not his.** They were quoted to show the
> *pattern*, not to be copied. **Never publish that this firm offers a service without Shimon
> confirming it does** — Rule 7, and misrepresenting the services of a regulated practice is the
> exact failure mode this site's rules exist to prevent.
>
> **What implementing it involves.** Ask him what the firm genuinely does within each service, then
> name those things. The existing "What it covers" lists are the right place.

#### I17. Add an FAQ page.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **What the other site does.** An FAQ block on its About page.
>
> **Value here.** Answers the questions a prospective client asks before they will call — fees, what
> switching accountants involves, what is needed to get started, how contact works during filing
> season. Also the natural home for questions the firm gets asked repeatedly by phone.
>
> **What implementing it involves.** A new page in the existing template. Questions and answers from
> Shimon; **fee and engagement answers in particular are his alone.**

#### I18. Add an insights or articles section.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **What the other site does.** A "Latest Insights" area alongside case studies, with reading times
> attached.
>
> **The honest caution to give him.** This is the highest-ongoing-cost idea on the list. An articles
> section with three posts from two years ago actively damages credibility — worse than not having
> one. **Raise the maintenance commitment with him before building it**, and consider whether the
> existing Due Dates and Track Your Refund pages already serve the "useful resource" role at zero
> upkeep.
>
> **What implementing it involves.** A listing page, a post template, and a standing commitment to
> publish. This is a static hand-built site with no content system, so each post is a hand-edited
> page unless something changes.

#### I19. Add a free tool or calculator.

**✅ DONE 2026-09-02 — realised by item 16.** A working compound interest calculator is live, with a
Financial Calculators landing page built to take more. The idea has been acted on; the remaining
calculators are tracked as items 17 and 18, not here.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **What the other site does.** Offers calculators as a footer resource.
>
> **Relevant precedent already here.** Track Your Refund and Tax Return Due Dates are exactly this
> kind of thing and are the most genuinely useful pages on his site. This idea extends a pattern
> that already works rather than starting something new.
>
> **⚠️ Accuracy constraint.** A calculator published by a CPA firm that produces a wrong number is a
> professional problem, not a bug. Anything numeric needs Shimon's sign-off on the arithmetic and
> a visible "estimate only, not advice" line. Cross-check against `terms.html`, which already
> disclaims the site as general information only.

#### I20. Add a "what happens next" section explaining the first thirty days.

**✅ DONE, LIVE 2026-09-24, commit `e7e156c`.** The getting started section replaced "Simple from day one" on the home page. **The wording is Shimon's own**, approved line by line after he rejected the first draft as *"for a bookkeeping firm"*. The pills were dropped because only step one had anything true to put in them. Checked live at desktop and phone width. See DECISIONS.md.
*The notes below are from before it shipped. The four unconfirmed claims in the warning (other than the free call, which he confirmed) did **not** ship. Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

**🟡 MOCKUP BUILT AND SEEN 2026-09-11. He likes the direction and wants it refined before it
goes anywhere near the site.** This idea is no longer just an idea; it is a design waiting on two
things from him. It is still I20 rather than a new item, because it is this item made concrete.

**Where the mockup lives — do not rebuild it from scratch:**

- `C:\Users\Admin\Documents\outputs\getting-started-section-mockup.html` — the working page
- `C:\Users\Admin\Documents\outputs\getting-started-mockup-desktop.png`
- `C:\Users\Admin\Documents\outputs\getting-started-mockup-phone.png`

Built from a reference he sent: three steps, a dark numbered circle each, a thin line joining them,
and a small outlined pill on each saying when or how often that step happens. Rebuilt in the firm's
own cream, gold and serif rather than the reference's colours. **It replaces the existing "Simple
from day one" block on the home page**, which is the same idea with three bare lines and no
timeframes.

**⏸️ What is outstanding, and who it has to come from:**

1. **The fine tuning. He has not said what it is.** He said only that it needs some. **Do not guess
   at it and do not start adjusting things on a hunch** — ask him what he wants changed.
2. **Every claim in the wording has to be confirmed by him.** See the warning below, which is the
   more serious of the two.

**One deliberate departure from his reference, not yet ruled on.** The reference puts the heading top
left; every other section on his site uses a centred heading with a small gold eyebrow above it. The
mockup follows **his site's centred convention**, borrowing only the reference's two-tone heading and
short gold rule, which his hero already uses. **He has not said which he prefers.** Switching to left
aligned is a few lines if he wants the reference exactly.

> **🚨 THE WORDING IN THE MOCKUP IS CLAUDE'S, NOT SHIMON'S. NOTHING IN IT IS CONFIRMED.**
>
> He asked for draft copy and that is what it is: plausible wording for a CPA firm, written to show
> the shape of the section. **It contains four statements about how the firm actually operates, and
> every one of them is an assertion a client could hold the firm to.** Rule 7. Each needs his yes
> before this is published:
>
> 1. **That the first call is free.** The pill reads "No charge".
> 2. **That setting a client up takes about two weeks.** The pill reads "First two weeks".
> 3. **That a client gets one named point of contact**, not a queue.
> 4. **That something arrives every month** — the copy says books kept current and a plain English
>    summary of where things stand.
>
> **Any of those that is not true cannot go on the site**, and the fix is his words, not a better
> paraphrase of mine. This is exactly what the original note below warned about: *do not describe an
> onboarding process the firm does not follow.*

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current state.** The home page has a three-step "Simple from day one" block — Reach out / We
> handle it / Stay ahead. It is the right idea at the wrong resolution: three short lines, no
> specifics, no timeframes.
>
> **What it removes.** The main reason a prospective client hesitates is not knowing what they are
> committing to. Naming what happens in week one, what the firm needs from them, and when they hear
> back removes that.
>
> **What implementing it involves.** Expanding the existing block rather than a new section. Shimon
> supplies the actual process — **do not describe an onboarding process the firm does not follow.**

### ACTION

#### I21. Use one primary button everywhere instead of several competing ones.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Measured.** The other site's home page has **40 links total** and one primary action — "Book Your
> Call" — with services using a clearly secondary "Explore More". His has **51 links** and competing
> calls: "Book a call" (gold), "Explore services" (ghost), "Client Login" (dark), all in the hero and
> header at once.
>
> **The insight worth relaying.** His page has *more links but less content* — the extra links are
> navigation scaffolding, not substance. More choices at the top of a page reduce the chance of any
> one being taken.
>
> **What implementing it involves.** Deciding which single action matters most and demoting the
> others visually. Note Client Login serves existing clients, not prospects, so it is a legitimate
> separate thing — **the competition is between "Book a call" and "Explore services."**

#### I22. Make that button open a real calendar with bookable slots.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **This is already item 4 in OPEN, and it is Shimon's own instruction, not an idea.** Do not treat
> it as a separate piece of work or raise it with him twice. Recorded here only so the ACTION group
> reads completely. Item 4 carries his exact words, the open decisions, and the portal
> cross-reference.
>
> **The comparison detail that belongs to it:** the other site embeds Calendly inline on a
> `/consultation` page for a named 30-minute discovery call. Item R1 has the specifics.

#### I23. Give every service block its own link through to its page.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **🛑 THIS ITEM WAS WRONG AS ORIGINALLY WORDED — CHECKED AND CORRECTED 2026-08-27.** The site
> **already does this.** All six service cards on the home page are `<a>` elements wrapping the whole
> card, each pointing at its own page (`services/tax-preparation.html` and so on); every card carries
> a "Learn more →" cue; no service is mentioned anywhere without a link. Verified on the live site.
> This also matches what Audit B found — every internal link resolves. **Do not "implement" this.**
>
> **What was actually observed, and all that survives.** The other site gives each service block a
> visually distinct **"Explore More" button**. His uses a "Learn more →" text cue inside an
> otherwise-plain card. The only real residue is *presentational* — whether the card looks obviously
> clickable — and that is a minor styling question, not a missing link.
>
> **➡️ UPDATE, 2026-08-27 — the residue is now a live request. See M24.** Shimon was told this item
> was already done, and that the only thing left in it was the button styling. **He then asked for
> exactly that**, in his words: *"we have to make a learn more button."* That is now **M24** in the
> MOTION section.
>
> **So the two entries do not contradict each other — read them as one story:**
> - **I23 (this item) — the FUNCTION. Closed, verified, nothing to build.** The cards link. They
>   always did.
> - **M24 — the APPEARANCE. Open, requested by him.** The "Learn more" text becomes a real button.
>
> **If Shimon asks about this one:** the link was never broken, and the button he asked for is
> tracked as M24. Do not tell him this item is outstanding, and do not close M24 on the grounds that
> this one is done.

#### I24. Add a closing call to action at the bottom of every page.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current state — partly present already, check before proposing.** The home page ends with the
> "Let's talk" band. The six service pages have a "Ready to get started?" panel, but it sits in the
> **sidebar**, which on a phone falls to the bottom anyway. The gap is on `tax-due-dates.html`,
> `track-refund.html`, `privacy.html` and `terms.html`, which end with the footer and no invitation
> — though Due Dates and Track Your Refund do each carry an inline "Let's talk" / "reach out" link
> mid-page.
>
> **What implementing it involves.** Reusing the existing "Let's talk" band on the pages that lack
> it. Low effort, existing components, no new design. Depends on item 4 / I22 being resolved first —
> **adding more routes to a dead contact form makes item 2 worse, not better.**

### DETAILS

#### I25. Put the full address on the site — suite number and ZIP included.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **This is the same change as item 8 in OPEN** — one job, not two. Item 8 has the detail of where
> the address appears and its two inconsistent spellings.
>
> **The comparison evidence.** The other site's footer carries a complete address —
> "33 Bartlett St, Suite 204, Brooklyn, NY 11206" — with phone and email. His shows
> "65 S 11th Street, Brooklyn NY", no ZIP, no suite. Seeing them side by side is what makes the
> incompleteness obvious.
>
> **Claude does not know the ZIP or whether there is a suite number — ask him, never guess.**

#### I26. Add a short line under each service saying who it suits.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current state.** Each home-page service card has a one-line description of the service. Each
> service *page* already has a "Who it's for" section — so the content largely exists, it just isn't
> surfaced where someone is choosing.
>
> **What implementing it involves.** A short second line on each of the six home-page cards, drawn
> from the "Who it's for" text already written. Cheap, and it makes the card grid scannable by need
> rather than by service name. Watch card height — six cards each gaining a line lengthens the
> section noticeably on a phone.

#### I27. Give the phone number more prominence in the header.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: website comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current state.** `(347) 486-2780` appears in the footer of every page and in the contact panels,
> correctly linked as `tel:+13474862780` — but **not in the header at all**, on any page or any
> screen size.
>
> **Why it matters more than it sounds.** While the contact form is dead (item 2), the phone is one
> of only two working ways to reach the firm — and it is currently below the fold on every page.
> Older and less patient visitors look for a phone number in the top right corner first.
>
> **What implementing it involves.** Adding it to the header, which is already crowded on desktop
> (brand, five nav items, two buttons) and collapses to a burger on mobile — so this needs a real
> layout decision, not just an insertion. Rule 2 preview, and it touches all twelve pages.

### REJECTED — do not raise these again

Shimon considered these and said no on **2026-08-27**. Recorded so no future Claude proposes them
back to him as fresh ideas.

- **Put the team on the site with photos and names.** Rejected.
- **Show a photo of the actual office.** Rejected.
- **Name the industries you serve.** Rejected — in his words, **"we serve everyone."**

**The consequence that bites later:** the comparison site's whole advantage comes from picking one
industry and letting every section inherit it. He has ruled that route out. **Any differentiation
proposed under I5 or I7 must therefore rest on something other than sector** — need, situation,
service model, or responsiveness. Do not reintroduce the industry angle in a new costume.

---

## MOTION — giving the site more life

**Added 2026-08-27.** Shimon's words: *"has much more things going on — things float in, numbers
count, there's a circle in the middle when you scroll down, things fade away. There's a lot of
interesting things. My website has really nothing, the only thing is that things fade in. That's it.
I wanna give it a little more life, a little more excitement."* He pre-approved adding all of this to
the list.

**Numbered M1–M24** so they never collide with the problems in OPEN (1–15) or the ideas in IDEAS
(I1–I27). **M24 is last at his request** — it is his own addition, not one of mine.

**Two subsections follow the items:** things deliberately *not* being copied from the other site, and
decisions only he can make. Neither is work.

**Standing rule applies to all of it:** every one of these changes how the site looks, so under
Rule 2 in `CLAUDE.md` each gets an HTML preview before it is built. **Nothing here is approved to
build** — it is approved onto the list.

> **📎 SHARED CONTEXT FOR THE WHOLE SECTION — read once, then the per-item blocks.**
> *Source: motion comparison against schapiracpa.com, 2026-08-27.*
>
> **What the other site actually runs.** GSAP, **Lenis** (momentum/smooth scrolling), Framer Motion,
> and a **Spline** 3D viewer. Measured live: 22 animations running at once, 108 elements carrying a
> transform, 211 carrying a transition. Its CSS keyframes are `marquee`, `marquee-infinite`,
> `spin-slow`, `fadeIn`, `slideUp`, `scroll-team`, `scroll-partners`, `fadein-slideup`,
> `hero-coin-in`, `hero-glow-pulse`, `spin`, `pulse`, `childcare-popup-in`.
>
> **The specific effects, identified:**
> - **The circle he mentioned** = a 128px ring with text set around a circular SVG path
>   (`animate-spin-slow`), turning continuously at **20s per revolution**, sitting ~2,437px down the
>   home page in the "Let's Build Something Bigger" band.
> - Testimonial **marquee**, 80s infinite loop. Partner-logo **marquee**, 40s. Team row auto-scroll
>   on the About page.
> - Gold coin in the hero: entrance animation plus a continuous glow pulse.
> - A **lead-capture modal** (`childcare-popup-in`, 400ms) offering a free loan-capacity check.
>
> **⚠️ The counters are UNVERIFIED.** He said "numbers count." The case-study figures
> ($1,200,000 / 23.4% etc.) are plain static `<span>`s with no counter markup and no data
> attributes — if they animate, it is driven inside React. **The audit could not trigger them**: the
> browser pane does not composite, which throttles the scroll animations needed to fire them. Treat
> counting as his observation, not as established fact.
>
> **What his site has today, measured.** **Zero CSS keyframes.** One scroll effect — `.reveal`,
> `opacity 0→1` plus `translateY(18px→0)` over 0.6s, fired by an IntersectionObserver at threshold
> 0.1 — applied **identically to all 22 blocks**. Plus 14 hover rules and 11 transition rules:
> `.btn` lift, `.card` lift with border and shadow, `.card .ci` icon fill, `.photo img` 1.045 scale
> over 1.1s, dropdown fade, caret rotations, footer link colour. `scroll-behavior:smooth` on `html`.
> Zero external scripts.
>
> **The diagnosis worth keeping.** He is right that it reads as nothing, but the cause is not that
> there is too little — it is that **the one effect he has is used the same way in all 22 places**.
> Same direction, same distance, same duration, same easing. Variety and staggering will buy more
> life than any new trick. Say this if he asks why the plan leads with the boring items.

### FOUNDATION

#### M1. Make every block visible by default and let the motion play on top, so the page still works when scripts don't run.

**✅ DONE 2026-08-27 — shipped in commit `4fd195e`, as the same fix as item 5.** Marked closed
2026-09-02 under the automatic-closing rule; it had been built and left open. Re-verified in
`assets/site.css` on 2026-09-02: every hide-then-animate rule is gated on `html.js-motion`, so with
scripting blocked the page renders complete and static.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **🔗 SAME FIX AS ITEM 5 IN OPEN — BUILT ONCE, ON 2026-08-27. Do not build it again.**
> Shimon approved item 5 and it was implemented in that one change; M1 is satisfied by it. The
> implementation: a one-line script in each page's `<head>` adds `js-motion` to `<html>` before the
> page paints, and every hide-then-animate rule in `assets/site.css` is now gated on
> `html.js-motion`. No script, no class, nothing hides — the page renders complete and static.
> Verified both ways in a browser: with scripting blocked every block and every heading child sits at
> full opacity; with scripting on the animation behaves exactly as before.
>
> **This is item 5 in OPEN, reframed as the enabler for everything below it.** Item 5 has the
> evidence: with scripting off, all 22 `.reveal` blocks sat at opacity 0 and the home page rendered
> as a blank cream screen.
>
> **Why it leads this section.** Every animation added on top of the current pattern deepens an
> existing fault. Adding M2–M23 without M1 means more of the page depends on scripts running, not
> less. **If Shimon wants only one thing from this section, it is this one.**
>
> **What implementing it involves.** Invert the default: `.reveal` visible, with an `is-animated`
> class added by script that opts the element *into* starting hidden. Then a no-script visitor sees a
> complete static page and everyone else sees the motion. The `prefers-reduced-motion` block already
> in `assets/site.css` is the working precedent for the same shape.

#### M2. Keep the existing reduced-motion setting so anyone who turns off animation sees a still page.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Already correct — this is a "don't break it" item, not a build.** `assets/site.css` has
> `@media(prefers-reduced-motion:reduce)` resetting `.reveal` to `opacity:1;transform:none;
> transition:none` and disabling the photo and brand transitions. Verified present on the live site.
>
> **Why it is listed.** Every new effect in M3–M23 must be added to that block at the same time.
> Motion sickness and vestibular disorders are real, the setting is a genuine accessibility
> requirement, and it is trivially easy to add an animation and forget the exemption.
>
> **What implementing it involves.** Nothing now; a checklist line on every later motion change.

#### M3. Pick one speed and one easing curve and use them everywhere.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current state.** Durations are scattered — 0.12s, 0.15s, 0.16s, 0.18s, 0.2s, 0.6s, 1.1s — with no
> shared easing; most rules use the browser default.
>
> **Why it matters more than it sounds.** A site whose movements share a rhythm reads as designed; one
> with a dozen unrelated timings reads as assembled. This is the cheapest single thing that makes
> motion feel intentional.
>
> **What implementing it involves.** Define two or three duration tokens and one easing curve in
> `:root`, then reference them. Invisible individually, noticeable in aggregate. Do it **before**
> M4–M23 so everything after inherits it.

### SCROLL

#### M4. Vary the entrance direction instead of one identical fade for all 22 blocks.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **The core fix of this whole section.** Every `.reveal` currently rises 18px and fades over 0.6s —
> all 22, identically. Sameness is what makes it disappear.
>
> **What implementing it involves.** Variant classes on top of `.reveal`: text blocks from below, side
> images from the side, full-width bands fading with a slight scale. Keep it to **three variants at
> most** — more becomes noise. Depends on M1 and M3 being done first.

#### M5. Stagger the six service cards so they arrive in sequence, not all at once.

**✅ DONE 2026-08-27 — shipped in commit `6ff76b3`.** Service cards now arrive in an even sequence.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Partly present already — check before proposing.** `assets/site.css` already staggers via
> `transition-delay` on `.grid .card:nth-child(2)` through `:nth-child(6)` (0.08s–0.26s), and on the
> trio and steps blocks.
>
> **So the real work is tuning, not building.** The delays exist but the effect is weak because all
> six cards also share the identical 0.6s fade-up from M4. Fix M4 first and this may need only a
> longer stagger interval.

#### M6. Make entrances shorter and quicker so the page feels responsive rather than sluggish.

**✅ DONE 2026-08-27 — shipped in commit `6ff76b3`.** Entrances shortened to 0.4s and 14px.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current.** 0.6s duration, 18px travel. That is slow for an entrance — the eye arrives before the
> content does, which reads as lag rather than polish.
>
> **What implementing it involves.** Roughly 0.35–0.45s and 12–14px travel. Counter-intuitive but this
> makes the site feel *more* animated, not less: quick motion registers as responsiveness, slow
> motion as waiting. Fold into the M3 token work.

#### M7. Bring headings in a beat before their body text.

**✅ DONE 2026-08-27 — shipped in commit `6ff76b3`.** Headings land a beat before the text beneath them.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current.** `.head` is a single `.reveal`, so the eyebrow label, heading and paragraph all arrive
> together as one lump.
>
> **What implementing it involves.** Split the reveal onto the child elements with a small delay
> between them — the same `transition-delay` mechanism already used for the cards, so no new
> machinery. Applies to the four section heads on the home page and the page heroes elsewhere.

#### M8. Start each entrance slightly earlier so nothing is still blank at mid-screen.

**✅ DONE 2026-08-27 — shipped in commit `6ff76b3`.** Entrances start just before an element reaches view.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current.** The IntersectionObserver uses `{threshold:.1}` with no `rootMargin`, so an element must
> be 10% inside the viewport before it starts. On a fast scroll the visitor reaches content that has
> not begun animating.
>
> **What implementing it involves.** Add a `rootMargin` with a **positive** bottom value so the
> observer's box extends below the viewport and elements start animating just before they enter view,
> and drop `threshold` to 0 so a tall block does not have to be 10% inside before it begins.
> Two values in the existing observer. **This also reduces the visible harm of item 5** if M1 has not
> shipped yet.
>
> **⚠️ Correction, 2026-08-27.** An earlier version of this block said to use a *negative* bottom
> value. **That was wrong and would have made it worse** — a negative `rootMargin` shrinks the
> observer's box and makes elements trigger *later*, which is the opposite of the intent. Positive
> grows the box downward and triggers earlier. Verified while building the preview.

### NUMBERS

#### M9. Count the key figures up as they scroll into view.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **⚠️ The other site's counters were NOT verified** — see the shared block at the top of this
> section. Build this because it suits a numbers business, not because their site provably does it.
>
> **Nothing to count yet.** The site currently has no firm statistics anywhere. **M10 must come
> first** or there is no content for this effect.
>
> **What implementing it involves.** A small script counting to a target on first view, once per
> visit. Ease the count and keep it under a second — a slow counter is irritating rather than
> impressive.

#### M10. Add a short strip of firm figures — years in practice, clients served, returns filed.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **The one item in this section that does two jobs.** It is the motion he asked for *and* it is
> evidence — the gap identified in the IDEAS section. Of everything in MOTION, this is the item that
> makes the site more credible rather than just livelier.
>
> **⚠️ Shimon supplies every figure and they must be true.** This is a regulated practice publishing
> claims about itself — Rule 7. Do not estimate, round up, or infer a client count from anything in
> the practice-manager app. **Ask him.** Listed as a decision at the end of this section.
>
> **What implementing it involves.** A three- or four-figure band, most naturally near the existing
> trust seals on the home page.

#### M11. Keep the final number in the page so it reads correctly if the count never runs.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **The M1 principle applied to counters.** Write the true final value into the markup and let the
> script count *from* a lower number *to* the value already there — never start from an empty element
> and fill it in. A no-script visitor then sees the real figures instead of blanks or zeros.
>
> **Why it is its own item.** This is the single most common way counters are built wrong, and getting
> it wrong on a page of firm statistics means publishing zeros about the practice.

### HOVER

#### M12. Animate the service icons rather than just recolouring them.

**✅ DONE 2026-08-27 — shipped in commit `4fd195e`.** Icon lifts and grows on hover. DESKTOP ONLY - no hover on a phone.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current.** `.card:hover .ci` swaps the circle to a gold fill with white icon over 0.18s. It works;
> it is just static in shape.
>
> **What implementing it involves.** The icons are inline SVG, so stroke-draw, a slight rotation or a
> scale are all available without new assets. **Desktop only in effect** — there is no hover on a
> phone, so this does nothing for most of his visitors. Rank it accordingly.

#### M13. Draw an underline in under text links.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current.** `a{text-decoration:none}` site-wide; nav links change colour only, footer links change
> colour over 0.12s.
>
> **What implementing it involves.** A pseudo-element underline scaling from 0 to full width on hover.
> Cheap and it reads as considered. **Do not remove the colour change as well** — colour alone is not
> a sufficient link affordance, and colour plus underline is better than either.

#### M14. Slide the arrow on "Learn more" to the right on hover.

**✅ DONE 2026-08-27 — shipped in commit `4fd195e`.** Arrow slides 4px on hover. DESKTOP ONLY - no hover on a phone.
*Left in place so its context block stays findable. Listed in DONE at the foot of this file.*

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current.** `.more` renders "Learn more →" as static text inside the card link, with no hover
> movement of its own.
>
> **➡️ UPDATE 2026-08-27 — approved by Shimon, built for preview, and it does NOT conflict with M24.**
> Checked before building: M24 keeps `.more` as a `<span>` styled to look like a button (it cannot
> become a `<button>` or a second `<a>`, because the whole card is already a link — see M24). The
> arrow therefore stays a child of `.more` either way, so **M14 does not need redoing when M24
> lands.** The one thing to revisit at that point: the slide distance is 4px, which may want reducing
> once the arrow sits inside a bordered button so it does not crowd the edge.
>
> **How it was built.** The arrow is wrapped so it can move on its own —
> `Learn more <span class="arw">→</span>` — with `display:inline-block` and a 4px slide on hover.
> **Verified the resting layout is unchanged**: width, height, position, font, weight and colour all
> identical to three decimal places with and without the wrapper.
>
> **Desktop only.** There is no hover on a phone, so most visitors will never see it.

#### M15. Give buttons a pressed state so clicks feel physical.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current.** `.btn:hover` lifts 1px with a shadow. There is **no `:active` state anywhere** on the
> site.
>
> **Why it is worth more than it looks.** `:active` is one of the few motion effects that works on a
> phone — it fires on tap. Most of this section is desktop-only; this one reaches his majority
> audience.
>
> **What implementing it involves.** An `:active` rule dropping the lift and softening the shadow. Two
> lines. **Best effort-to-value ratio in the HOVER group.**

### AMBIENT

#### M16. Add one slowly rotating circular badge with the firm name around it.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **This is the effect he specifically asked for** — "there's a circle in the middle when you scroll
> down." Their version: 128px, text on a circular SVG path, `animate-spin-slow` at 20s per
> revolution, one instance only.
>
> **What implementing it involves.** An SVG `<path>` circle with `<textPath>`, rotated by a CSS
> keyframe. No library needed. **Once, in one place** — the whole effect depends on scarcity, and it
> must go in the reduced-motion exemption since it never stops.
>
> **Judgement to pass on if asked.** This is the most decorative item on the list and the one most
> capable of looking cheap if overdone or badly placed. Their single instance works; three would not.
> The wording matters more than the motion — a rotating ring saying something vacuous is worse than
> no ring.

#### M17. Let the hero photo drift a little as the page scrolls.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **What implementing it involves.** A small parallax offset on `.photo img` driven by scroll
> position. The image is already absolutely positioned inside a fixed-ratio frame with
> `object-fit:cover`, so there is headroom to move it without exposing an edge.
>
> **Keep it very small** — a few percent. Parallax is the effect most likely to read as a template
> site, and it is a common motion-sickness trigger, so it must sit inside the reduced-motion
> exemption. Scroll-linked, so it needs throttling to avoid jank on a phone.

#### M18. Add a soft glow behind the CPA seal so the trust row has a focal point.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Their equivalent.** `hero-glow-pulse` behind the gold coin.
>
> **Current state here.** `.cpabadge` is a flat gold circle with an inset ring. The trust band reads
> evenly — nothing draws the eye.
>
> **What implementing it involves.** A soft radial glow, either static or on a slow pulse. **Cross-check
> item 6 and Question B first** — the seal already fails contrast, and drawing attention to a
> membership claim that has not been confirmed current makes an unverified statement more prominent.

#### M19. Add a slow ribbon of client quotes, once there are real quotes to put in it.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Blocked on I2** — the site has no testimonials at all. This is a container with nothing to put in
> it until Shimon gathers quotes and permission to publish names.
>
> **What implementing it involves.** A CSS marquee, duplicated track, `animation-play-state:paused` on
> hover so a reader can actually read one. Their loop is 80s. **Must pause under reduced-motion**, and
> a moving block of text is genuinely hard to read — consider whether a static row serves better.

### NAVIGATION

#### M20. Shrink the top bar slightly after the first scroll.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current.** `header` is `position:sticky;top:0` at a fixed 79px with a blurred translucent
> background. It never changes.
>
> **⚠️ Touches item 14.** The header height is exactly what puts anchored sections behind the bar. A
> header that changes height makes the `scroll-margin-top` fix in item 14 harder, not easier —
> **resolve item 14 first, or do both in one change.**

#### M21. Add a thin progress line at the top of long pages.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Where it earns its place.** Only the home page (6,648px on mobile) and the legal pages are long
> enough to benefit. On short pages it is decoration.
>
> **What implementing it involves.** A 2–3px bar pinned under the header, width driven by scroll
> position. Cheap. Modern CSS scroll-driven animations can do it without script, which suits the M1
> principle — but browser support needs checking at build time.

#### M22. Fade the mobile menu items in one after another.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current.** `.mmenu.open` switches straight to `display:block` — the whole menu appears instantly
> with no transition at all.
>
> **Why this one is worth doing.** It is one of the few items in this section that **most of his
> visitors will actually see**, since the mobile menu is the primary navigation on a phone. The audit
> confirmed the menu itself is well built — this is polish on something already working.
>
> **What implementing it involves.** Staggered delays on the menu children. Note `display:none` cannot
> be transitioned, so the open state needs restructuring slightly.

#### M23. Add a back-to-top button once the visitor is well down the page.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: motion comparison
> against schapiracpa.com, 2026-08-27.*
>
> **Current.** No such control. The header is sticky, so the nav is always reachable — this is a
> convenience, not a fix.
>
> **What implementing it involves.** A fixed button appearing past a scroll threshold, fading in.
> `html{scroll-behavior:smooth}` is already set so the scroll itself is free. **Keep it clear of the
> footer links** flagged as small tap targets in item 11, and give it a real accessible label.

### THE BUTTON

#### M24. Turn the "Learn more" line on each service card into a real button.

> **📎 CONTEXT FOR CLAUDE** — *reference material, not to be read out. Source: **Shimon's own
> request**, 2026-08-27, in his words: **"we have to make a learn more button."** Placed last at his
> request.*
>
> **🔗 READ THIS WITH I23 — they are not contradictory.** I23 in the IDEAS section is marked *already
> done*, and it is: **the links work.** All six service cards are `<a>` elements wrapping the whole
> card, each pointing at its own page. Nothing is missing or broken.
>
> **The distinction, and why both entries stand:**
> - **I23 was about function** — "does each service block link through to its page?" **Yes. Closed.
>   Do not build it.**
> - **M24 is about appearance** — the cue is currently `<span class="more">Learn more →</span>`,
>   styled as plain gold text inside the card. The other firm uses a visible "Explore More" button.
>   **Shimon has now asked for the button.** That makes it an open piece of work.
>
> When I23 was closed on 2026-08-27 the button styling was explicitly named as the only surviving
> residue of it. **He has now asked for exactly that residue.** So: the link was never the problem,
> the styling is the request.
>
> **What implementing it involves.** Restyle `.more` as a button — most simply by reusing the existing
> `.btn.ghost` treatment so it matches the rest of the site rather than introducing a new component.
>
> **⚠️ One real constraint.** The whole card is already a single `<a>`. **A `<button>` or a second
> `<a>` cannot be nested inside it** — nested interactive elements are invalid HTML and break keyboard
> and screen-reader navigation. Two valid routes: style the existing `<span>` to *look* like a button
> while the card stays the link, or unwrap the card and make only the button the link. **The first is
> far less disruptive** and keeps the whole-card click target, which is better on a phone. Pair with
> M14 for the arrow movement.

### NOT DOING — deliberately rejected from the other site

Recorded so nobody proposes them later as improvements. These are Claude's judgements, not Shimon's
decisions — **he can overrule any of them.**

- **Their pop-up offering a free loan check** (`childcare-popup-in`) — an interstitial like that
  cheapens a professional firm and is the most aggressive thing on their site.
- **Their momentum scrolling** (Lenis) — fights the phone's native scroll feel and is a common
  accessibility complaint.
- **Their 3D hero object** (Spline) — heavy, slow, and the wrong register for an accounting practice.
- **Their multiple looping marquees** — one is a flourish, four is a fairground. M19 keeps at most
  one.
- **Fading content out as it scrolls away** — he mentioned liking "things fade away", but this removes
  text while someone is still reading it. **If he asks for it specifically, that is his call** — but
  raise the readability cost first.

### DECISIONS NEEDED — his call, not a build

**➡️ Moved 2026-08-27 into OPEN QUESTIONS as D, E, F and G**, so they are tracked the same way as
every other question only Shimon can answer. Listed here as pointers only — **the detail lives with
the questions, do not duplicate it back into this section.**

- **Restrained or lively?** → **Question D.** Sets M3, M6 and how much of AMBIENT is built.
- **Which firm figures will he publish?** → **Question E.** Blocks M9, M10 and M11 entirely.
- **What does the rotating badge say?** → **Question F.** Blocks M16.
- **Before or after the contact form and domain?** → **Question G.** Partly answered — he approved
  M5–M8 for immediate build on 2026-08-27.

---

## DONE

Finished work, newest first. **Items stay in their original section above as well**, so the
📎 context blocks behind them remain where a future Claude will look. This is the index.

### Shipped 2026-09-24

**Commit `b34c761`: the Financial Calculators page redesign goes live.** Direction C, bold dark,
with one drawing per card and no corner icon. The closing panel shows the phone number and email
directly, because the Contact page's form still sends nothing (item 2). The live file was confirmed
identical to the commit and checked at desktop and phone width.

- **26.** The calculator cards should be a graphic, not words: *realised as the whole-page redesign*

**Commit `62492e1`: the calculators page header goes cream.** He found the dark header too much and
out of keeping with the site, and chose the lightened version of the same layout (option H2).
Nothing else on the page changed. Live file matches the commit, checked at desktop and phone width.

- **26, follow-up.** Replace the dark header band

**Commit `f8c1c55`: the three calculator pages get a designed header and a closing panel.** He
chose the pale drawing header; the closing panel is the light version. The calculators give
identical results on 13 test cases before and after. Live files match the commit, checked at
desktop and phone width.

- **30.** Give each calculator page a header with some design to it, plus *"the book a call box on bottom"*

**Commit `e7e156c`: the getting started section goes live on the home page.** It replaces "Simple
from day one", uses Shimon's approved copy word for word, and has no pills. The live files were
confirmed identical to the commit and checked at desktop and phone width.

- **I20.** Add a "what happens next" section: *realised as the getting started section*

### Shipped 2026-09-11

**Commit `213dfbb` — Calculator 10, the break even calculator, goes live.** Published at
`break-even-calculator.html` with a third card on the Financial Calculators page. Arithmetic verified
against a separate implementation on 58 cases before publishing.

- **28.** Break Even Calculator — calculator 10

### Shipped 2026-09-03

**Commit `76d83eb` — Calculator 2, the mortgage payment calculator, goes live.** Published at
`mortgage-calculator.html` with a second card on the Financial Calculators page. No number in the
address, per the convention settled the same day. The arithmetic was verified independently against
the standard amortisation formula and cross-checked against MoneyGeek's calculator before publishing.

- **17.** Calculator 2 — monthly mortgage payment
- **H.** Should the big figure be the loan repayment or the full monthly cost — *answered: full cost*
- **I.** Does he approve the line under the heading — *answered: yes, as drafted*
- Three items from **27** built and shipped: the full monthly cost headline, the year by year
  schedule, and hovering the chart for principal and interest

**Commit `b8e0153` — Shimon's own wording for the line under the calculator's heading.** Used
character for character. Longer than what it replaced, so the hero is taller; nothing was adjusted to
compensate, at his instruction.

- **24.** Change the description on the compound interest calculator

**Commits `d412475` → `808f119` — clicking the calculator chart does nothing, so the black box is
gone.** Rule 2's preview requirement was waived by Shimon for this one change; it is back in force for
everything after it. `808f119` narrowed the fix after he insisted nothing but the click behaviour
change — `d412475` had also restyled the keyboard focus ring and added fallback listeners, and both
were taken back out.

- **21.** A black box appears around the whole chart when you hover over it

### Shipped 2026-09-02

**Commits `626d9ab` → `66d8bac` — the Financial Calculators feature.** Four commits in quick
succession, because two sessions collided mid-deploy and garbled text was briefly live. Independently
re-verified against the live site on 2026-09-02: all 15 pages load, titles are clean, the menu entry
appears exactly once on desktop and phone, the calculator's arithmetic is correct, nothing regressed
on the 13 older pages, and the published files match what is committed.

- **16.** Calculator 1 — savings growth (compound interest)
- **I19.** Add a free tool or calculator — *realised by 16*
- **A menu item to reach them** — settled as an entry inside Resources, not a new top-level heading

### Closed 2026-09-02 — finished earlier, never marked

Found by the first sweep under the automatic-closing rule. Both were built and shipped on 2026-08-27
and simply never crossed off.

- **M1.** Make every block visible by default and let the motion play on top — *shipped in `4fd195e`
  as the same fix as item 5*

### Shipped 2026-08-27

**Commit `4fd195e` — six approved fixes.** Preview approved for the four visual ones first.

- **5.** The whole site disappears if a visitor's browser blocks scripts
- **7.** One state's refund link is dead, and about a dozen don't land where the page promises
- **9.** A mistyped or out-of-date link shows a blank white page
- **12.** A few wording and punctuation slips
- **M12.** Animate the service icons rather than just recolouring them.
- **M14.** Slide the arrow on "Learn more" to the right on hover.

**Commit `6ff76b3` — four scroll-timing changes.** Preview rule waived by Shimon for that one
change only; it is back in force for everything after it.

- **M5.** Stagger the six service cards so they arrive in sequence, not all at once.
- **M6.** Make entrances shorter and quicker so the page feels responsive rather than sluggish.
- **M7.** Bring headings in a beat before their body text.
- **M8.** Start each entrance slightly earlier so nothing is still blank at mid-screen.

**⚠️ M12 and M14 are desktop-only.** Both fire on hover and there is no hover on a phone, so
most visitors will never see them. Shimon was told this before approving. Do not present them
later as mobile improvements, and do not wire them to tap — a tap follows the card link.

### Questions answered

- **A.** Does info@hirsch.cpa reach a monitored mailbox? — **Yes** (2026-08-27). Closed.
- **B.** Are the AICPA and NYSSCPA memberships current? — **Yes** (2026-08-27). Closed.
  Unblocks I4 and M18, which were held back pending this.
- **D.** Restrained or lively? — **partly answered** ("could be better"). Still open; see the
  question for what is still needed.
