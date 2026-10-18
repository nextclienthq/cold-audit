# cold-audit

A Claude skill that turns a prospect's website into a reason to reply.

Give it a prospect's URL and it checks their public online presence — website, tracking, ads, proof, lead response — and picks the **three costliest problems the prospect can verify themselves**. Then it writes:

- a one-page audit you can send as-is
- a cold email, a LinkedIn note and message
- three follow-ups (day 3, 7 and 14)
- a private "behind the audit" list: unused findings, what it couldn't check, and how sure it is

Every finding comes from something it actually saw, with where to check. No invented numbers, no guessed load times, no "your website is terrible".

## What makes it different

- **Lead response check.** Most audits stop at the website. cold-audit also looks at what happens after someone gets in touch: response-time promises, out-of-hours coverage, lead magnets that collect nothing.
- **Tracking checked on the loaded page,** not the raw HTML, and it knows the difference between "no pixel" and "pixel waiting for cookie consent".
- **Template leftovers.** It spots logo strips and placeholders that quietly cost a business its credibility.
- **Self-check.** It stops if the "prospect" turns out to be your own company or a current client.

## Install

**Claude.ai (web, desktop, mobile)**
1. Download `cold-audit.zip` from this repo.
2. Upload it as a skill in Claude, then turn it on under **Customize > Skills**. Code execution must be enabled.
3. In a chat: *"/cold-audit https://prospect.com — I sell Meta ads"*

**Claude Code**
Copy the `cold-audit/` folder into `~/.claude/skills/`, then ask Claude to audit a prospect.

Works best when Claude has a browser (for example Claude in Chrome): tracking checks and the Meta Ad Library need one. Without it, those sections are marked "unverified" instead of guessed.

## Files

```
cold-audit/
├── SKILL.md                  # the workflow
├── references/checks.md      # what to check, and priorities by service you sell
└── assets/audit-template.md  # the one-page audit
```

## License

MIT — use it, change it, sell your audits with it.

---

Made by [Next Client](https://clientedit.substack.com) — helping agency owners find their next clients.
