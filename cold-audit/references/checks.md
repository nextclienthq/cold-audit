# Checks

Part 1 is what to look at on any prospect. Part 2 is what to prioritise for the user's lens.

## Part 1 — What to look at

### First screen
- In five seconds, can a stranger tell **what they sell, who it's for, and why them**? Or is it a slogan?
- Is there **one obvious next step**, or several buttons competing, or none?
- Does the first screen sell the main offer, or a side tool (a free checker, a newsletter) that attracts the wrong visitors?
- On a phone: are call / book / WhatsApp reachable without opening the menu?

### Offer
- Concrete offer (package, starting price, timeline, what's included) or only "contact us"?
- If prices are hidden, is there a reason to get in touch (free call, quote in 24h, guarantee)?
- Services described by the **result for the buyer**, or by process and features?

### Proof
- Testimonials with real names and companies? Recent?
- Case studies with numbers or a before/after?
- Big claims ("500+ projects", "trusted by…") backed by anything a buyer can check?
- **Template leftovers:** logo strips of famous brands, stock team photos, placeholder text. Check the page code: image file names that don't match their labels (e.g. a "Circle" logo that loads a big-brand file) are a strong sign of a template that was never cleaned up. Phrase it as "looks like leftover placeholders", never as an accusation.

### Lead response
- What response time does the site promise? Do different sections promise different things?
- Out of hours: is there anything that answers (booking, chat, voice agent, auto-reply), or does the lead wait?
- Contact form: how many fields, which are required, does it say what happens next?
- Lead magnet (audit tool, guide, calculator): does it ask for contact details, and is anything set up to follow up?
- Phone number clickable on mobile? WhatsApp present and linked?

### Freshness and trust
- Blog or news: date of the last post.
- Footer copyright year, outdated events, broken links, placeholder copy, mismatched languages (e.g. an Italian placeholder on an English form).
- About page: real people, or anonymous?

### Tracking (only from the loaded page)
Load the page in a browser, wait ~3 seconds, then run:

```js
const html = document.documentElement.outerHTML;
({
  metaPixel: /fbq\(|connect\.facebook\.net/.test(html) || typeof window.fbq === 'function',
  ga4: [...new Set(html.match(/G-[A-Z0-9]{6,12}/g) || [])],
  googleAds: [...new Set(html.match(/AW-\d{6,}/g) || [])],
  gtm: [...new Set(html.match(/GTM-[A-Z0-9]{4,10}/g) || [])],
  linkedin: /snap\.licdn\.com/.test(html),
  tiktok: /analytics\.tiktok\.com/.test(html),
  consentTool: /cookiebot|onetrust|iubenda|cookieyes|complianz|usercentrics/i.test(html)
})
```

- No tags **and** no consent tool → tracking is genuinely absent. Strong finding, especially if the site claims to be data-driven.
- No tags **but** a consent tool → tags may be waiting for consent. Not a finding unless you accept cookies and they still don't appear.
- Running ads with no pixel → they pay for traffic they can't measure or retarget.

### Speed (only from PageSpeed data)
- Mobile performance score and Largest Contentful Paint. Below ~50, or LCP above ~4 s, is worth raising — in terms of visitors who leave.

### Ads (only from Ad Library / Transparency Center)
- Filter by the advertiser's page name; keyword searches mix in unrelated brands.
- Active ads? How many, how long running, how many variations?
- Do they send people to the homepage or a dedicated page?
- Does the ad promise match the landing page?
- Does the advertiser run ads for something other than its main business? Note it — it can reveal what really pays their bills.

### Search
- Page 1 for "[main service] [city/niche]"? Who appears instead? (Only if you can see Google's own results.)
- Google Business Profile: present, photos, hours, reviews answered?

### LinkedIn (if it loads)
- Company page: last post, followers, clear description.
- Founder: headline says what they do for whom? Active or silent?

## Part 2 — Priorities by lens

Pick what the user can credibly fix. A web designer pitching a missing pixel sounds off-brand; an ads specialist pitching it sounds expert.

**Paid ads**
1. Ads running (or the business clearly depending on ads) with no pixel or conversion tracking.
2. Ads sending people to the homepage or a page with no clear offer.
3. Competitors advertising visibly while the prospect isn't.
4. A lead magnet or decent traffic with no way to retarget.
5. One creative running for months, or a single variation.

**Lead response & automation**
1. Contradictory or missing response-time promises.
2. Nothing answers out of hours: no booking, chat, voice agent or auto-reply.
3. Lead magnet that collects nothing, or collects contacts with no visible follow-up.
4. Only manual contact paths (phone in office hours, generic email).
5. Long or vague forms with no "what happens next".

**Website & conversion**
1. First screen doesn't say what they sell and to whom.
2. No single next step, or it's hard to find on a phone.
3. Weak, missing or template-looking proof.
4. Form friction and no expectation set after submitting.
5. Slow mobile (from PageSpeed only).

**SEO**
1. Not on page 1 for the main service + location; name who is.
2. One generic services page instead of a page per service or location.
3. Dormant blog while competitors rank with content.
4. Weak Google Business Profile.
5. Slow mobile (from PageSpeed only).

**Content & social**
1. Blog or social channels dormant (give the last post date).
2. LinkedIn inactive while competitors post.
3. Clients exist but no client stories are shown.
4. Social profiles not linked from the site, or broken links.
5. Message on the site doesn't match the social profiles.

**General** — take the three strongest from any area, favouring first-screen clarity, lead response and proof: they apply to almost every business and the prospect sees them instantly.
