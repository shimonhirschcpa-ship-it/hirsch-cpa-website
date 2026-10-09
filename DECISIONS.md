# DECISIONS — hirsch.cpa website

**What this file is.** The append-only record of every change made to the website and **why**. Newest
entries go at the top, under the horizontal rule.

**Why it exists.** The markup shows *what*. The history shows *when*. Neither shows *why this and not
the obvious alternative* — and on a site where most choices are judgement calls about how a
professional firm should present itself, the reasoning is the only thing that stops the next Claude
undoing a deliberate choice because it looked like an oversight. **The purpose of this file is that a
future Claude understands the thinking, not just the code.**

**Started:** 2026-08-26, at Shimon's instruction. Changes made before this date are not recorded
here.

---

## HOW TO WRITE AN ENTRY

Copy this shape. **Shimon supplies the reason; Claude writes it down.** Never invent a reason to fill
a field — if you don't know why you're making a change, that is the signal to stop and ask.

```
### Short title — what changed

**When:** YYYY-MM-DD · **Commit:** <sha, or "this commit">

**What changed:** one or two plain sentences.

**Why — in Shimon's words:** his reason, as he gave it. Not an improved paraphrase.

**Was a preview approved?** Yes / not a visual change. (Rule 2 — a look-and-feel change is not
started until he has approved a preview of it.)

**What could break, and why:** which other pages share this; whether any published statement stops
being true because of it. "Nothing" is an acceptable answer ONLY if you actually looked.

**Conflicts with an existing rule?** Name the rule and say why the change is right anyway — or say
"None" if there genuinely is none.

**How it was checked:** which pages were opened and looked at, including at phone width.

> **This is Shimon's decision. No Claude may change it on its own initiative.**
```

The three bold questions — **why**, **what could break**, **does it conflict** — are not optional.
They are the whole point of the record. See [CLAUDE.md](CLAUDE.md) Rule 5.

---

## ENTRIES

### Calculator pages: a header with each calculator's own drawing, and a closing panel

**When:** 2026-09-24 · **Commit:** `f8c1c55` (closes item 30)

**What changed:** on the compound interest, mortgage and break-even pages, two things.
- **The header.** The site's standard centred cream band is replaced by a cream band with:
  - a "← Financial Calculators" link back to the index
  - the title on the left, with "Calculator" in gold italic
  - the page's own intro paragraph, unchanged
  - **that calculator's own drawing, large and faint on the right**. It is the same drawing as its card on the Financial Calculators page.
- **The closing panel.** Each page now ends with the "Questions about *your results?*" panel after its "estimate, not advice" note: the same wording and button as the index, with the phone number and email shown as working links.

The calculators themselves are untouched.

**Why, in Shimon's words:** *"now make the headers on each calculator page better with some sort of design like you did here. send me screenshots."* Then *"and also the book a call box on bottom."* He was shown two directions on all three pages. **He chose the pale drawing over the large medallion** (the drawing in a dark circle).

**Why the closing panel is light, not dark like the index's:** under the calculator, the dark panel competed with the results and chart. It became the heaviest thing on the page and pulled the eye from the result figure, which is the point of the page. The light version is a white card with a thin gold left edge, which echoes the gold edge of the "estimate, not advice" note above it. Both versions were built and compared before he saw the light one.

**The rule for new calculators:** a new calculator page uses **its card drawing as its header drawing**, so there is nothing new to design. Drawings for Retirement, S-corp vs LLC and Penalties & Interest already exist: open `outputs\calculators-page-C-bold-dark-v2.html` with `?n=6` in the address and copy the drawing from the card.

**Was a preview approved?** Yes: `outputs\calc-header-pale-drawing-{compound-interest,mortgage,break-even}.html`, with desktop and phone pictures. The live pages were built from the same code.

**Deliberately different from the index:** the index keeps the chart pattern and cards overlapping its header. The calculator pages have neither, so the index still reads as the parent page.

**Left alone, flagged:** the index's closing panel also reads "Questions about *your results?*", which is odd on a page with no results. **He has not been asked about it. Do not change the index without his say so.**

**What could break, and why:**
- *The maths.* Only the header section, one new section before the footer, and new style rules changed; no script was touched. **Proved rather than assumed:** 13 test cases (5 compound, 4 mortgage, 4 break-even) were run on the live pages before the change. Each captured every result, message and the first and last row of every table. The same cases were run again locally before committing and on the live site after it published, and gave **identical results all three times**.
- *Style clashes.* These pages already use class names like `.k`, `.v` and `.row` in their results. All of those rules are scoped inside the results area, so none reach the new panel. The new classes (`.chd`, `.ccl`) are used nowhere else. The shared `.phero` was not changed, so every other page keeps its header.
- *The phone first screen.* The header is shorter than before on a phone, so the first input box sits higher.
- *Published statements.* The Contact page's form still sends nothing (item 2), so the panel shows the phone number and email directly. The privacy policy is unaffected: no scripts or forms were added.

**Conflicts with an existing rule?** None.

**How it was checked:** all three live files were confirmed identical to the commit. On each live page, at 1440 and at 375 wide:
- no sideways scroll and no console errors
- the new header drawing present and the old header gone
- the back link going to the Financial Calculators page
- the phone number and email as working links
- no em dash visible anywhere
- the first input on the first screen: its bottom edge at 502 to 559px on a 812px phone screen

> **This is Shimon's decision. No Claude may change it on its own initiative.**

---

### Financial Calculators page: cream header in place of the dark one

**When:** 2026-09-24 · **Commit:** `62492e1` (follow-up to `b34c761`, item 26)

**What changed:** only the header band at the top of the Financial Calculators page. It is now the site's cream instead of near-black. The title is dark ink with "calculators" in dark gold italic. The faint chart pattern stays, redrawn in pale gold so it reads on cream, and there is a thin line under the band, as on other pages. The layout is unchanged: the title sits on the left, the chart on the right, and the cards still overlap the band's bottom edge. **Nothing below the header changed:** the cards, "Before you start" and the dark closing panel are exactly as shipped in `b34c761`.

**Why, in Shimon's words:** *"the black header background is too much, doesn't match with the rest of the site. The cards are good."* **He rejected the dark header as not matching the rest of the site.** He was shown three light options: H1, the other pages' plain cream band; H2, the same layout lightened; and H3, a deeper sand with a centred title. **He chose H2, the lightened version of the same layout.**

**Was a preview approved?** Yes: `outputs\calculators-header-H2-cream-with-chart.html`. The live header was built to the same values as that mockup.

**On the dark closing panel:** Claude's view was that it still works once the header is light, because it matches the dark panels on the cards. The question was put to him with the three options. He asked for nothing else to change, so it stays. **Do not lighten it without his say so.**

**What could break, and why:** the change is eight lines in this page's own style block and three colour values in its chart drawing. No shared styles, no other page, no wording. The privacy policy is unaffected.

**Conflicts with an existing rule?** None. Rule 3 held: he said the cards are good, and nothing else was touched.

**How it was checked:** the live file was confirmed identical to the commit. On the live site:
- *Desktop, 1440 wide:* cream header with the pale chart, three cards in a row overlapping its edge.
- *Phone, 375 wide:* cards stacked.
- *Both widths:* no sideways scroll, no console errors, no em dashes.
- *Each card:* exactly one medallion drawing in its dark panel, and no corner icons.
- *Closing panel:* still dark, with the phone number and email as working links.

> **This is Shimon's decision. No Claude may change it on its own initiative.**

---

### The Financial Calculators page redesigned: bold dark, one drawing per card

**When:** 2026-09-24 · **Commit:** `b34c761` (closes item 26)

**What changed:** the whole Financial Calculators page. The old version was a cream band with a title and one line, three white text cards, then the footer. The new page has:
- a dark header with a faint gold chart pattern behind the title
- three cards that overlap the bottom of that header, each leading with a single gold drawing on a dark panel
- a "Before you start" section (free, private, an estimate not advice)
- a closing dark panel with the phone number, the email and a "Book a free call" button

**Why, in Shimon's words:** on the cards, from item 26: they should be *"primarily a large graphic or icon with the calculator's name, not words"*. On the page: *"it looks very blah now"*, then *"Not only the cards, the whole page is too plain."* He picked the dark preview-panel cards from three card styles and asked for two changes. First, use the drawing from the round medallion version in the panel. Second, remove the small icon in the corner, which was his original complaint. Looking at the whole page with those changes, he said *"perfect, push live"*.

**Was a preview approved?** Yes. There were three card styles, then three whole-page directions, then the revised page C (`outputs\calculators-page-C-bold-dark-v2.html`). He approved that last one as shown.

**The wording on the page is Claude's draft, which he approved by approving the page as shown.** Recorded line by line so it does not pass unnoticed. **New wording:**
- Eyebrow "Resources"
- The heading as "Financial *calculators*", with "calculators" in gold italic (the old heading was "Financial Calculators")
- "Good to know" / "Before you start"
- "Free to use" / "Every calculator here is free. There is nothing to sign up for."
- "Private by design" / "They run entirely in your own browser. The figures you type are not sent to us and are not saved."
- "An estimate, not advice" / "Each result is based only on the figures you enter. Your own situation may be different."
- "Questions about *your results?*" / "Book a free call and we'll go through them with you."
- The button label "Book a free call"

**Carried over unchanged:** the line under the title, the three calculator names and their descriptions, and "Open calculator". The two headings "Free to use" and "Private by design" were not his wording before today. Every claim in them was checked as true: the privacy policy's calculator paragraph says the same thing, "An estimate, not advice" is on every calculator page, and he confirmed the free call earlier the same day. **"We'll go through them with you" is a promise about the firm's service. He approved it as shown; it is his to change.**

**The faint chart pattern behind the header title stays deliberately.** Claude raised whether it should go, given his "one graphic per card" comment. He did not answer that point and approved the page as shown. **Do not remove it on your own initiative.**

**What could break, and why:**
- *Other pages.* All the new styling lives in this page's own style block under names used nowhere else on the site. The home page's `.card`, which the old cards used, is untouched, and the shared stylesheet was not changed. The page uses the shared `.trio`, `.head`, `.tag` and `.btn` classes as they are, without restyling them.
- *The Contact page.* The "Book a free call" button leads to the Contact page, whose form still sends nothing (item 2). **That is why the closing panel also shows the phone number and email directly**, so nobody hits a dead end. When item 2 is fixed, nothing here needs to change.
- *Published statements.* The privacy policy stays true (standing rule on item 3): the page adds no scripts, no tracking and no form, and the calculators still send nothing.
- *More calculators.* Cards centre and wrap: three across, four as two and two (a rule that switches on automatically when there are exactly four), five as three and two, six as three and three, and one per line on a phone. **When a new calculator is added, copy a card, draw its own gold icon to match the others, and keep one drawing per card with no corner icon.**

**Conflicts with an existing rule?** None. Rule 3 was the live risk, since a whole-page redesign invites touching the shared stylesheet, so nothing shared was changed.

**How it was checked:** built from the approved mockup's own code, not retyped. The page shell (header, menu, footer, scripts) is unchanged. Tested locally, then on the live site after it published. The live file was confirmed identical to the commit.
- *Desktop, 1440 wide:* three cards in one row.
- *Phone, 375 wide:* three cards stacked full width.
- *Both widths:* no sideways scroll, no console errors, no em dashes.
- *Each card:* exactly one drawing, sitting in its dark panel, and no corner icons anywhere on the page.
- *Closing panel:* the phone number and email are shown as working links.

> **This is Shimon's decision. No Claude may change it on its own initiative.**

---

### The home page's getting started section, in Shimon's own words

**When:** 2026-09-24 · **Commit:** `e7e156c` (closes idea I20)

**What changed:** the home page's "Simple from day one" block is replaced by the getting started section from the mockup: a heading reading "Getting started *is simple*" under a short gold line, then three dark numbered circles joined by a thin line, each with a step heading and a short paragraph. On a phone the steps stack and the line is hidden. The styles went into the shared stylesheet under new names, the same way the calculators were built. Nothing else on the page changed.

**Why, in Shimon's words:** the only words of his relayed to this session were his verdict on the first draft, that it read as written *"for a bookkeeping firm"*. He rejected that draft, then went through the replacement copy line by line and cut an em dash and a phrase he disliked. **The words now on the page are his, approved line by line, and are used exactly as he left them.** He confirmed the free call is accurate. The previous draft's other claims (a two week setup, a single point of contact, something delivered every month) were never confirmed and are gone. **They must not come back without his say so.**

**The pills were dropped.** Each step in the first draft had a small outlined label saying when or how often that step happens. Only step one had anything true to say ("free call"). Steps two and three only ever had made up timeframes, and anything else would either repeat the heading or be new wording he hadn't approved. So all three came out rather than leave one standing alone.

**Was a preview approved?** Yes. The mockup with his approved copy and no pills (`outputs\getting-started-section-mockup-v2.html`, desktop and phone pictures alongside) was shown first, and he approved it before anything touched the site.

**What could break, and why:**
- *Other pages.* The new styles are shared, but every name is new and used only on the home page, with one exception. `.head em` (the gold italic in the heading) would restyle any section heading on any page that contains italic text. At the time of this change no other heading has any, which was checked.
- *The old styles.* The old step styles are no longer used on the home page. They were left in the stylesheet, not tidied away (Rule 3).
- *Published statements.* The privacy policy is unaffected because the section collects nothing. The one factual claim is the free call, which he confirmed.

**Conflicts with an existing rule?** One judgement call against "keep the design exactly". The mockup showed the section on cream, but on the real page the sections directly above and below are already cream, so the section keeps the lighter background the old block had and the page keeps alternating. The circles, line, type and spacing are exactly the mockup's. **If he wants it on cream, that is a one-word change: flag it to him, don't decide it.** Also, on phones this section's heading is 31px rather than the 30px other section headings use, as in the mockup. That rule applies to this section only.

**How it was checked:** tested on a local copy first, then on the live site after it published. The live home page and stylesheet were confirmed identical to what was committed. On the live site at 1440px wide: three columns, joining line showing, all three steps visible. At 375px: steps stacked, line hidden, no sideways scroll. No console errors at either width. The old block is gone, the text matches his copy character for character, and there are no em dashes anywhere on the page.

> **This is Shimon's decision. No Claude may change it on its own initiative.**

---

### A third view on the compound interest calculator — principal against interest

**When:** 2026-09-15 · **Commit:** `df9c046` (closes item 22)

**What changed:** a third icon joins the bars and the table on the compound interest calculator. It draws two lines across the years, what has been paid in and what it has earned, each shaded down to the baseline. On a long enough run they cross, at the year the interest overtakes the contributions.

**Why — in Shimon's words:** *“I want line 1. Principle 2. Interest so at one point it crosses”*, with two reference images of the same chart from another firm's calculator, the second showing its hover box.

**Was a preview approved?** Yes. A standalone mockup was built first and revised four times on his instruction before anything touched the real page: the crossing marker came off, the description text came out of the hover box, the ahead/behind line came out, and the dots came off the lines at rest.

**What could break, and why:** the view is additive — the bar chart, the year by year table and every figure on the page are untouched, and all three were re-checked after the change. It shares the page's own stylesheet and the site shell, so nothing on any other page is affected. No published statement stops being true: **the privacy policy's claim that the calculators run entirely in the browser still holds, because this view sends nothing anywhere** — checked, per the standing rule on item 3.

**Conflicts with an existing rule?** None. Rule 3 was the live risk — a third view is exactly the kind of change that invites tidying the other two on the way past — and nothing else on the page was touched.

**How it was checked:** the real page opened at desktop and at 375px. Three views switch cleanly; the line redraws when the figures change and when the window resizes; the year by year table is intact on all three calculators; nothing in the new view is focusable or clickable; no console errors; no sideways scroll on a phone and all three icons 44px. The figures were checked against a separate model built from scratch — principal, interest and the balance they sum to, matching to the dollar.

> **This is Shimon's decision. No Claude may change it on its own initiative.**

---

### Four fixes: phone headings, the copyright year, the footer, the privacy policy

**When:** 2026-09-15 · **Commit:** `68b9eda` (closes items 3, 14, 15, 19)

**What changed:** tapping About or Services on a phone no longer lands the section heading behind the bar that stays at the top. The copyright year now keeps itself right. Financial Calculators was added to the footer Resources list on all 17 pages, directly under Due Dates. The privacy policy was rewritten so it describes what the site actually does.

**Why — in Shimon's words:** he approved all four by name off the outstanding list, and on the footer said the link should sit **under Due Dates**.

**Was a preview approved?** Not a visual change — three are behaviour or text, and the footer addition follows the existing list exactly.

**What could break, and why:** **the real risk here was the year.** The three calculators already use `table.yr` for the year by year schedule, so a `.yr` class on the copyright year would have let the setter overwrite those tables with a four digit number. It is `js-year` for that reason, and the schedules were re-checked on all three calculators afterwards. The literal year stays in the markup so the page still reads correctly with scripts off. **The privacy rewrite is the opposite risk** — it is a statement a regulated practice is accountable for, so every claim left in it was checked against the site itself.

**Conflicts with an existing rule?** None. Rule 7 is the reason the privacy rewrite happened at all.

**How it was checked:** all 17 pages carry the year setter and the footer link, exactly once each. The scroll fix measured on a phone viewport: the About eyebrow lands 105px below a bar whose bottom is at 78px, where it used to sit behind it. The four false claims are confirmed gone from the policy.

> **This is Shimon's decision. No Claude may change it on its own initiative.**

---

### Clicking the chart now does nothing, so the black box around it is gone

**When:** 2026-09-03 · **Commit:** this commit (closes item 21)

**What changed:** on the compound interest calculator, clicking the chart no longer does anything at
all. Hovering still highlights a year and still clears when the pointer leaves. The thick black
rectangle that used to appear around the whole chart is gone.

**Why — in Shimon's words:** *"clicking a bar currently locks it highlighted and draws a black line
around the whole chart. He doesn't want clicking to do anything at all. Only moving the cursor over a
bar should highlight it, and it should clear when the cursor leaves. No click behaviour, so the black
line never appears."* He was explicit that it be removed properly — *"remove the click-to-lock
entirely, not just hide the outline."*

**What it actually was — worth recording, because the diagnosis was not what the symptom suggested.**
There was **never a click handler.** The chart is covered by one transparent overlay that spans the
whole plot area, carrying `tabindex="0"` so the arrow keys can step through the years. Clicking it
gave it *focus*, and two things followed: the `focus` handler lit up a year and left it lit, and the
browser drew its default focus ring — which, because the overlay covers the entire chart, reads as a
box around the whole thing rather than around one bar. So "click-to-lock" and "the black line" were
one mechanism, not two. **Do not go looking for a click listener to delete; there isn't one.**

**How it was fixed:** the focus ring is suppressed on `:focus` and restored on `:focus-visible`, and
the `focus` handler now highlights only when the focus came from the keyboard. `:focus-visible` is
the selector browsers use to tell a keyboard apart from a mouse. A fallback watches whether the last
input was Tab or a pointer, for browsers that don't support it.

**Was a preview approved?** No preview was built. **Rule 2 was waived by Shimon for this change** —
he described the end state himself, in detail, and instructed "test it, then deploy". The rule is
back in force for everything after it.

**What could break, and why:**
- **Nothing else on the site shares this.** Both the CSS and the JavaScript are inside
  `compound-interest-calculator.html`, in that page's own `<style>` and `<script>`. No other page has
  a chart. `assets/site.css` was not touched, so the other fourteen pages are byte-identical.
- **Phones were the real risk and were checked first.** Removing click behaviour could have left
  phone users with no way to read a year's figures, since there is no hover on a phone. It does not:
  taps are handled by separate `touchstart`/`touchmove` listeners that never involve focus, and they
  were tested working after the change. The table view is a second route to the same numbers. **No
  loss on mobile.**
- **Keyboard access is intact and was the constraint that shaped the fix.** The overlay's own label
  tells a screen-reader user the arrow keys work. Removing `tabindex` would have killed the black box
  too — and made that statement untrue, which Rule 7 forbids. The arrow keys still step through the
  years and the focus ring still appears for keyboard users, in the firm's gold.
- **The arithmetic was not touched.** No change to any calculation, the layout, the sizes or the
  fonts — he was emphatic about that. The default result is still $29,542.

**Conflicts with an existing rule?** **Rule 2** (preview before building a visual change) — waived by
him for this change, as recorded above. Rule 7 pointed the other way and was the reason the keyboard
outline was kept rather than deleted outright.

**How it was checked:** driven in a browser before deploying — a click (nothing shown, no outline), a
hover (year highlighted, others dimmed), the pointer leaving (cleared), a real Tab press (gold
outline, year highlighted, arrow keys stepping), and a simulated tap (year shown). The gold could not
be confirmed in the local file because the shared stylesheet does not load over `file://`; it was
confirmed by supplying the variable, and again on the live page after deploying.

> **This is Shimon's decision. No Claude may change it on its own initiative.**

---

### Two defects in the calculator pages as first published — titles and a doubled menu line

**When:** 2026-09-02 · **Commit:** `f5c7aac` (fixes `626d9ab`)

**What changed:** Both new pages went live at `626d9ab` carrying two faults. Their browser-tab titles
read **"Financial Calculators u{00B7} Hirsch CPA"** and **"Compound Interest Calculator u{00B7}
Hirsch CPA"** — raw escape text where the separator dot belongs — and the same fault was in the
og:title and twitter:title tags that fill in a link preview when the page is shared. Separately,
**"Financial Calculators" appeared twice** in the Resources dropdown on those two pages, on the
desktop menu and the phone menu alike. Both are now corrected. Nothing else on either page changed.

**Why — whose reason this is.** This is not a new instruction from Shimon; it is a defect fix against
his existing one. The standing requirements it serves are his: the calculator must be **exactly** the
version he approved on 2026-08-27, and the pages must carry the site's real top bar and footer with
**every link working** — which was the whole reason this work was held back from deployment the first
time round. A duplicated menu line and a garbled page title are the same class of fault as the 38
dead links: the firm's public face showing something no one intended.

**How both got out.** The two pages are assembled by a script rather than hand-typed, so that the
calculator's markup, CSS and script can be lifted byte-for-byte from the approved file. Two things
went wrong in that assembly, and the pages were committed and pushed by a second session that was
working in this repository at the same time, while the files were still mid-rebuild on disk.

- The script wrote the separator as a PowerShell unicode escape. **Windows PowerShell 5.1 does not
  support that form**, so the escape text itself was written into the file. Worth knowing for next
  time: this machine runs 5.1, not 7.
- The frame — top bar, menu, footer — was copied from the **working copy** of `tax-due-dates.html`,
  which by then already carried the new Resources line. The line was then added again on top. The
  frame is now taken from `4fd195e`, the commit before any calculator work, so it is added once.

**Was a preview approved?** Not a look-and-feel change. Nothing was designed here; two faults were
removed so that the pages match what Shimon already approved. The calculator's own markup, CSS and
script were verified byte-identical to the 2026-08-27 approved file both before and after.

**What could break, and why:** nothing else shares these two pages — they are the only files touched,
and the other thirteen pages were not opened. The `<title>` and the share-preview tags are per-page.
No published statement changed, so nothing that was true stopped being true. The one thing worth
watching is the reverse: while these two pages were wrong, anyone who shared a link to them would
have got a preview card with `u{00B7}` in the headline. That is now fixed, but a link shared during
that window may still show the old card until the sharing service re-reads the page.

**Conflicts with an existing rule?** **None.** Rule 3 was held strictly: only the two new pages were
touched. Rule 6 was honoured — the tree was committed before and after, and the rollback point is
`626d9ab`.

**On the arithmetic — the thing he actually asked to be sure of.** Checked independently rather than
taken on trust from the earlier session. The page's year-by-year loop was compared against the
standard future-value formulae, written out separately from scratch, across fifteen cases: the
reference case, zero starting amount, zero contributions, zero rate, one year, 120 years, 100% rate,
and the once-a-year contribution mode. Every case agreed to the dollar. The same sweep was then run
in a browser against the deployed page, eleven cases, checking each time that **the big number, the
chart and the table all say the same thing** and that the table's running totals add up to the final
figure. They do. The method — monthly compounding, money added at the end of each period — matches
the MoneyGeek reference formula, and the reference case was also worked through by hand, month by
month: $5,000 plus $150 a month at 4% comes to **$7,037** after one year, which is what the page
shows.

**One thing to put to Shimon, not a fault.** In the *once-a-year* contribution mode this page still
compounds monthly and simply adds the money once at year end. MoneyGeek switches to annual
compounding in that mode, so its answer is slightly lower. Neither is wrong — it is a modelling
choice, and keeping the compounding the same regardless of how often you contribute is the more
consistent of the two — but it is a real difference from the stated reference and he should know it
is there. Related: the field is labelled a rate "each year", and 4% compounded monthly grows 4.074%
in a year. Every mainstream calculator behaves this way. **No wording was changed on his behalf.**

**How it was checked:** the two pages were opened and driven in a browser, on the local copy and then
on the deployed site, at full width (1280) and at phone width (375). Confirmed: titles correct, the
Resources dropdown lists three entries once each on desktop and on the phone menu, the phone menu
opens and Resources expands and collapses, the card opens the calculator, the hero watermark and
brand mark load, no console errors, and no sideways scrolling at either width. The header and footer
were proved byte-identical to `tax-due-dates.html` as committed at `4fd195e`. Every internal link on
all sixteen live pages was fetched: **19 distinct targets, none broken.**

> **This is Shimon's decision. No Claude may change it on its own initiative.**

---


### Financial Calculators — a new Resources entry, a landing page, and the compound interest calculator

**Why the change is being made — his words.** He wanted calculators on the site but not another item
in the top bar: the top bar **"looks clogged."** So it goes inside the existing **Resources**
dropdown as a single line, **"Financial Calculators"**, which opens a landing page showing the
calculators as cards. One calculator today, built so adding three more is trivial.

On the calculator itself he set a hard condition: it must be **exactly** the version he approved on
2026-08-27 — **"same size, same fonts, same layout"** — because he had noticed a version that
rendered slightly smaller and wanted the bigger, approved one.

And before it went live he asked for the arithmetic to be proved, not asserted: **"I wanna make sure
that the calculator is actually accurate, that the numbers get calculated good... the calculation
behind the calculator when it calculates the numbers is good and accurate for compound interest. So
year and the monthly contribution and everything."**

**Why it was NOT deployed the first time it was asked for.** The preview files were mock-ups: the
landing page had **38 placeholder links that went nowhere**, and the approved calculator carried a
cut-down top bar with absolute links pointing back out to the live site. Publishing those as-is would
have put 38 dead links on the firm's public site and left one page with a top bar unlike the other
thirteen. That was put to Shimon rather than guessed at, and he approved rebuilding the frame.

**What was actually done.**

- The entry was added to the Resources dropdown, desktop and mobile, on all **13 existing pages**.
  The insert was scripted off the exact existing markup so the three link-prefix variants (root,
  `/` on 404, `../` under services) each got the right path. The **footer** Resources column was
  deliberately **left alone** — he asked for the dropdown, and Rule 3 says change only that.
- `calculators.html` is new, built from `track-refund.html` so its header and footer are the site's
  own markup verbatim rather than a re-typed copy.
- `compound-interest-calculator.html` is new. **The approved calculator's stylesheet, markup and
  script were carried over byte-for-byte.** Only the frame changed: the real site header and footer
  replaced the cut-down ones, the mobile menu was added, and the nav script came with it.

**What could break, and why.**

- *The calculator rendering differently from what he approved.* This was the whole condition, so it
  was proved rather than assumed. Its `<style>` block, its markup between the header and the footer,
  and its script were each compared character by character against
  `calculator-1-compound-interest-APPROVED-2026-08-27.html` and are identical — 23,331 characters of
  markup matching exactly once the newly added mobile-menu block is set aside. Its inline stylesheet
  was also confirmed to be an exact **superset** of `assets/site.css`, which is why the new header
  renders identically to every other page without linking the shared stylesheet and risking a
  cascade change. In the browser the page measured **1140px** of content width — its full design
  width, unchanged.
- *The "smaller" rendering he reported.* Traced and explained: the earlier preview showed the
  calculator inside a frame roughly **914px** wide, below its 1140px design width. The file was never
  at fault. Nothing needed fixing.
- *The maths being wrong on a CPA firm's public site.* See below.
- *Dead links.* Every local link on both new pages was checked to resolve to a real file. The only
  unresolved reference is `mortgage-calculator.html`, which sits inside an HTML comment as the
  template for the next card and is not a live link.

**How the maths was verified.** The `project()` function was extracted from the approved file itself
— not re-typed — and run against three independent references: the standard closed-form ordinary
annuity formula, a freshly written month-by-month loop, and a hand calculation printed month by
month. It is a monthly-compounding ordinary annuity: interest is credited first, then the
contribution is added at the **end** of each period. That is the conventional and conservative
choice, and it matches the MoneyGeek reference the page was modelled on — $5,000 plus $150 a month
at 4% gives **$7,037** after one year, which the page reproduces exactly.

Both contribution modes were tested (monthly and annual are different code paths), along with zero
initial amount, zero contributions, zero rate, one year, 120 years and 100% rate. Agreement with the
independent formulas is exact to the limit of double precision (worst relative difference 2.5e-15).
The chart, the table and the headline were confirmed to agree, and the table's running totals to
reconcile to the final figure, across **10.1 million** year-rows spanning every realistic input.

One thing was found and is recorded deliberately: because the page prints **whole dollars**, two
separately rounded figures can sum to $1 different from the rounded total. It cannot occur in any
realistic scenario — the smallest balance at which it is possible is about **$839 billion**, and it
needs something like 21% sustained for 62 years. The underlying figures are exact; only the rounded
display differs. It was reported to Shimon rather than silently fixed, because changing the rounding
would change a calculator he had approved byte-for-byte.

**Conflicts with an existing rule?** **No.** Rule 2 was honoured — he saw and approved the preview
before any of this was built, and approved the frame rebuild separately once the mock-up problem was
put to him. Rule 3 was held: the footer column and the thirteen pages' other content were left
untouched. Rule 6 was honoured — the tree was clean and committed before the change; the rollback
point is `4fd195e`. Rule 7 holds: nothing published stopped being true, and the calculator carries
its existing note that it is an estimate.

**Addendum — two defects went live briefly and were fixed the same evening.**

The first commit of this work (`626d9ab`) published the two new pages in a bad state. Neither defect
touched the calculator's own numbers, markup or styling, and no other page was affected.

1. **"Financial Calculators" appeared twice** in the Resources dropdown, on desktop and in the phone
   menu, on `calculators.html` and `compound-interest-calculator.html` only. The frame for those two
   pages was copied from a page whose working copy had already been given the new entry, and the
   entry was then added again on top.
2. **The page titles read `Financial Calculators u{00B7} Hirsch CPA`** — the escape text for the
   middot separator was written into the file instead of the character. This also reached the
   `og:title` and `twitter:title` share-preview tags.

Both were fixed in `f5c7aac` and `d2732a1`. The pages are now rebuilt from the site's own header and
footer, with the invariants **asserted before anything is written**: exactly one desktop and one
mobile link, no placeholder links, and the calculator's stylesheet, markup and script byte-identical
to the approved file. Verified on the live site afterwards: one entry in each menu, titles carrying
the same middot the other pages use, the calculator at its full 1140px width, the card centred on
desktop and fitting a phone with no sideways scroll, and the projection reproducing $7,037 for the
reference case with the table agreeing with the headline.

**The lesson worth keeping.** The original build was run twice in a row, and the second run read a
working copy the first run had already modified. A generator that reads the very files it writes is
not safe to re-run. The rebuild takes its frame from a known-good source and refuses to write at all
unless every invariant holds. **Do not "just re-run" a page generator against the working tree — check
what it reads, or make it assert.**

Related: the browser checks that were run before the first push confirmed the calculator's maths, its
width and the menu on thirteen pages, but counted *whether* the entry was present rather than *how
many times*, and read the page title only as a tab label. Both defects were inside what was looked
at and outside what was actually asserted. **Count, don't just check for presence.**

> **This is Shimon's decision. No Claude may change it on its own initiative.**

---

### Six approved fixes — no-script fallback, refund links, a 404 page, wording, card hover

**When:** 2026-08-27 · **Commit:** `4fd195e` (previous state `6ff76b3`)

**What changed:** six items Shimon picked off the list — items 5, 7, 9 and 12, plus motion items
M12 and M14.

- **Item 5 / M1 — the site no longer goes blank when a browser blocks scripts.** A one-line script
  in each page's `<head>` marks the page as able to animate, before it paints; every
  hide-then-animate rule is now conditional on that mark. No script, nothing hides. **This is the
  same underlying fix as M1 in the motion list — built once, and cross-referenced in both entries so
  nobody does it twice.**
- **Item 7 — refund links.** Maine was returning "403 Forbidden" and now opens the Maine Tax Portal
  refund form. Eleven others that dropped people on a state portal front page now go straight to the
  refund lookup: Arkansas, Delaware, Hawaii, Illinois, Indiana, Louisiana, Mississippi, Montana,
  Nebraska, Pennsylvania, Washington DC. **Oklahoma was deliberately left alone** — its refund
  lookup is a script inside the portal with no address to link to, and the pattern that worked for
  the other portals produced a broken empty page there, so the front page remains correct.
- **Item 9 — a real page for wrong links,** replacing a blank white page. Built from the site's own
  header, footer and styling, with root-absolute addresses (one 404 is served for wrong addresses at
  any depth, so relative ones would break) and `noindex`.
- **Item 12 — five punctuation and hyphenation corrections.** Two comma splices became full stops;
  "Year end" → "Year-end"; "Payroll set up" → "Payroll setup"; "Clean up of prior period books" →
  "Cleanup of prior-period books". No meaning changed, no dates or figures touched.
- **M12 — the service card icon now moves,** lifting 3px and growing 6% on hover, on top of the gold
  fill it already had.
- **M14 — the arrow after "Learn more" slides 4px right on hover.** The arrow is wrapped in a span so
  it can move independently.

**⚠️ M12 and M14 are DESKTOP-ONLY.** Both fire on hover, and **there is no hover on a phone** — so
most of the firm's visitors will never see either one. Shimon was told this plainly before he
approved them, in the preview and in the report. Do not later present them as improvements for
mobile visitors, and do not "fix" them by wiring them to tap: a tap on a card follows the link, and
hijacking that would break navigation.

**Why — in Shimon's words:** he selected these off the to-do list and approved the preview covering
items 9, 12, M12 and M14. His earlier standing instruction on the form and the site's plainness sits
behind items 5 and 12; the refund links came out of the design audit.

**Was a preview approved?** **Yes for the four visual ones.** Items 9, 12, M12 and M14 were built as
a standalone HTML preview and approved before anything was applied — Rule 2 followed in full. Items
5 and 7 have no visual result at rest, so they were built directly, which is why they are not in the
preview.

**What could break, and why:**

- *Item 5 inverts how every animated block behaves.* Verified both ways in a browser: with scripting
  blocked every block and every heading line renders at full opacity; with scripting on the animation
  is unchanged. The `prefers-reduced-motion` exemption was updated to match the new selectors in the
  same change.
- *M14 adds markup inside a line of text,* which risked shifting the layout. Measured: width, height,
  position, font, weight and colour identical to three decimal places with and without the wrapper.
- *The 404 page is served for wrong addresses at any depth.* Verified live at `/no-such-page`,
  `/services/nope` and `/a/b/c-missing` — all three return a real 404 status with the branded page,
  and its stylesheet and logo resolve.
- *External state links rot.* All 42 were opened in a real browser, not merely status-checked, and
  each lands on an actual refund form or refund page. **This is a measurement taken on 2026-08-27 —
  re-check before relying on it.**

Nothing published stopped being true. The only wording touched was punctuation.

**Conflicts with an existing rule?** **None.** Rule 2 was followed for the four visual items and does
not apply to the two invisible ones. Rule 6 was honoured — the tree was confirmed clean and the
rollback commit is `6ff76b3`. Rule 3 was held: the audit found plenty more worth fixing and none of
it was touched.

**How it was checked:** visible text compared against `6ff76b3` on all twelve pages — identical
everywhere except the four carrying approved wording edits, and those changed *exactly* as approved
and no further. Markup identical everywhere except the six wrapped arrows and the refund addresses;
un-wrapping the arrows programmatically restored the home page's markup to byte-identical. The
stylesheet was reversed edit by edit and confirmed byte-identical to `6ff76b3` once all four approved
CSS changes were undone. Icon and arrow confirmed motionless at rest and moving on hover. After
deployment: the live stylesheet matches the committed one, all thirteen pages return 200, all 42
refund links resolve, the wording is live, and forty computed properties across the home page match
the pre-change baseline exactly — page height 11,651px, body text 2,731 characters, 22 animated
blocks, all unchanged.

> **This is Shimon's decision. No Claude may change it on its own initiative.**

---

### Scroll entrance timing — four changes to how content arrives

**When:** 2026-08-27 · **Commit:** see below (the four motion items M5–M8)

**What changed:** only the timing and sequencing of the fade-in that already existed. The six service
cards now arrive one after another instead of in two uneven bursts; every entrance is quicker and
travels a shorter distance (0.6s/18px → 0.4s/14px); the heading in a section block arrives a beat
before the words under it; and everything starts moving slightly before it reaches the middle of the
screen instead of after. **Nothing at rest changed** — no words, fonts, sizes, colours, spacing or
layout.

**Why — in Shimon's words:** *"has much more things going on — things float in, numbers count,
there's a circle in the middle when you scroll down, things fade away. There's a lot of interesting
things. My website has really nothing, the only thing is that things fade in. That's it. I wanna give
it a little more life, a little more excitement."* He compared the site against schapiracpa.com,
picked four of the five Scroll items off the resulting plan, and instructed: *"Just for this time, I
wanna make an exception. Do not build me a HTML. Push it right away to the website and make sure that
absolutely nothing changes, but nothing except those four things."*

**Was a preview approved?** **No — Shimon explicitly waived Rule 2 for this one change**, in the
words quoted above. He was shown no preview because he asked not to be. **The waiver was for this
change only. Rule 2 is back in force for everything after it** — do not treat this as a precedent.

**What could break, and why:** the stylesheet is shared by all twelve pages, so a timing mistake
would show everywhere at once. Three specific risks were checked before pushing:

- *The heading change alters how a block animates.* `.head`, `.phero .wrap` and `.shero .wrap` no
  longer fade as one lump; their children fade in order instead. Verified that the resting state is
  identical — every child ends at full opacity with no transform — and that before the animation runs
  the block is invisible exactly as before.
- *Static pages.* `privacy.html` and `terms.html` deliberately have no scroll animation. Their
  `.phero .wrap` carries no `reveal` class, so the new rules do not match them. Verified untouched.
- *Reduced motion.* The new child rules would have stayed invisible for anyone who has asked their
  device to reduce animation. They were added to the existing `prefers-reduced-motion` exemption in
  the same change. Verified.

Nothing published stopped being true: no wording was touched.

**Conflicts with an existing rule?** **Yes — Rule 2 (show a preview before building).** Shimon
waived it himself, for this change only, in the words quoted above. Rule 6 (a way back) was honoured:
the tree was confirmed clean and the rollback commit is `08177cb`. Rule 3 was held strictly — the
audit found many other things worth fixing and **none of them were touched.**

**How it was checked:** the full diff was read line by line (13 files: the stylesheet plus one
identical line in each of the twelve pages). Visible text and markup were compared against `08177cb`
with script blocks excluded and found byte-identical on all twelve pages. Every stylesheet rule
outside the animation block was confirmed unchanged. The new rules were driven in a browser to
confirm the resting appearance, the new delay ladder (0, .08, .16, .24, .32, .40), the heading
sequence (0, .09, .18), that the trio and steps blocks kept their original delays, and that the
reduced-motion exemption covers the new rules. Computed styles for forty elements were captured
before the change and re-checked after deployment.

> **This is Shimon's decision. No Claude may change it on its own initiative.**

---

*Entries above this line are newest first.*
