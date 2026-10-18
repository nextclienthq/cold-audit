---
name: cold-audit
description: Audit a prospect's public online presence and turn the 3 costliest, verifiable problems into a one-page audit plus a cold email, DM and follow-ups. Use when given a prospect to pitch.
---

# Cold Audit

You help agency owners and freelancers start sales conversations by sending a prospect a short audit of their public online presence. The audit is not a report. It is a reason to reply: three problems the prospect can check for themselves in under a minute, explained in terms of lost money, each one pointing at what the sender sells.

Two rules decide whether this works:

1. **Nothing goes in that you didn't see.** Every finding comes from a page, a tool result or a search you actually ran, and you can say where. You never estimate load times, invent competitors, guess at ad spend or imply a tracking gap you didn't confirm. One false claim and the prospect stops reading — and remembers who sent it.
2. **Every finding is a business problem.** "Missing meta description" is a chore. "People who find you on Google see a vague snippet and click the next result" is a reason to talk.

## Step 0 — Make sure this is a real prospect

Before collecting anything, check that the prospect is not the user's own company, a sister brand, or a current client. Compare the company name, legal entity, address, ad account names and contact details with what you know about the user. If there is overlap, stop and ask. An audit of your own agency is still useful, but as an internal fix list, not as cold outreach.

## Step 1 — Inputs

Required: the prospect's website (or company name — then find the official site and confirm it if unsure).

Ask once, in one message, only for what's missing:
- **What the user sells** — this is the lens: paid ads · lead response & automation · website & conversion · SEO · content & social · general. If you already know it, don't ask.
- Optional: the prospect's LinkedIn and their main market or city.

If the user doesn't answer, use the general lens and the prospect's own country as market.

## Step 2 — Collect evidence

Keep a private **evidence log**: what you saw, where, and a confidence tag:
- `verified` — seen directly (page, code, tool result)
- `likely` — strong indirect signal
- `unverified` — couldn't access

Read `references/checks.md` before you start: it has the checks for each area and what to prioritise for each lens.

**A. Website (always).** Homepage plus up to four key pages: services, pricing, about, contact/booking, one case study or blog post. Note what a stranger understands in the first screen, how they take the next step, and what proof backs the claims.

**B. Tracking — check the loaded page, not the source.** Many sites inject tags with JavaScript, so raw HTML can miss them. If you have a browser, load the page, wait a few seconds and run the snippet in `references/checks.md`. If there's a cookie banner, note whether tags are held back until consent — "no pixel before consent" is correct behaviour, not a finding. Without a browser, mark tracking `unverified`.

**C. Speed.** Try the PageSpeed Insights API (mobile). If it fails, drop speed entirely. Never describe a load time you didn't measure.

**D. Ads.** Meta Ad Library: search the brand, then **filter by the advertiser's page name** — keyword results are full of unrelated brands. Note active vs. inactive, start dates, what the ads promise and where they send people. Google Ads Transparency Center the same way. If a source won't load, mark it `unverified`.

**E. Proof and reputation.** Testimonials, case studies, client logos, reviews (Google, Trustpilot, Clutch, G2 — whatever fits the market). Note numbers only when you see them. Compare with one or two direct competitors only if you actually find them.

**F. Lead response.** This is where most audits stop and most money is lost. Record what the site promises ("we reply within 2 hours"), whether those promises agree with each other, how someone contacts them out of hours, whether there is instant booking, chat or WhatsApp, and whether a lead magnet captures contact details. Never submit a form, start a chat or place a call yourself. If the user wants a real response-time test, they make a genuine enquiry as themselves and tell you what happened.

**G. Search and LinkedIn.** Search the main service + city the way a buyer would. Unless you can see Google's own results, mark rankings `unverified`. LinkedIn is usually behind a login — mark it `unverified` if it doesn't load.

Anything you couldn't access that matters for the lens goes on the "To complete" list at the end.

## Step 3 — Choose three findings

Score each candidate from 1 to 3 on:
- **Impact** — how directly it costs leads, sales or trust
- **Relevance** — how directly the user's offer fixes it
- **Checkability** — `verified` = 3, `likely` = 2, `unverified` = 0 (never used in the audit)

Keep the top three. On a tie, pick the one the prospect can see fastest.

Drop:
- advice that fits any website ("add more CTAs", "post more often")
- technical details with no business consequence, unless the lens is SEO and you tie them to lost traffic
- anything that sounds like a judgement of their taste, team or brand

Use only broad, well-known benchmarks, phrased generally. No made-up percentages.

## Step 4 — Write the audit

Use `assets/audit-template.md`.

- One page, three findings.
- Open with one specific, true compliment — proof you actually looked.
- Each finding: a headline stating the consequence in plain words · **What I saw** (specific, with where to check) · **Why it costs you** · **Quick fix** (one concrete action, useful on its own).
- Write for the owner, not a marketer. Explain any technical term in half a line.
- Tone: a peer who noticed something. Never alarmist.
- End with one low-pressure call to action tied to finding #1.
- Write in the language of the prospect's website unless told otherwise.
- Sign with the user's name and business, or leave placeholders.

## Step 5 — Write the outreach

All personalisation comes from the evidence log. No "I hope this finds you well", no "I came across your website".

- **Cold email** — subject of six words or fewer, specific to them. Body under 90 words: why them, the single sharpest finding, offer the full audit, end with an easy question.
- **LinkedIn** — connection note under 300 characters, plus a message for after they accept.
- **Follow-ups** — day 3 (finding #2), day 7 (finding #3 or a quick win they can do today), day 14 (short, polite close).

## Step 6 — Deliver

In this order:
1. **The audit**, ready to send.
2. **The outreach**: email, LinkedIn note and message, three follow-ups.
3. **Behind the audit** (for the user only):
   - findings you didn't use, with sources, so the user can swap one in;
   - **To complete** — what you couldn't access and the exact screenshot that would let you check it;
   - every finding tagged `likely`, and why.

If the user sends screenshots or more information later, update the log, re-score, and say which finding changed and why.
