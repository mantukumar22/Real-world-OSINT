# Module 09 — Legal & Ethical Boundaries (Read This Before Every Investigation)

> This module intentionally does **not** provide step-by-step instructions for
> illegal activity. Instead, it teaches you to recognize the legal line, cite
> the actual laws that apply, and understand real consequences — the same way
> a proper university or professional cybersecurity course (SANS, CompTIA,
> university CS-ethics curricula) covers "computer crime law" without teaching
> students to commit computer crime.

## 9.1 The Core Distinction

| Legal OSINT | Illegal Activity (Not OSINT) |
|---|---|
| Reading public posts/pages | Unauthorized access to private accounts/systems |
| Google dorking indexed public files | Exploiting a vulnerability to reach non-public data |
| WHOIS lookups | Using breach data to log into accounts |
| Reverse image search | Installing keyloggers/spyware on someone's device |
| Aggregating public facts for journalism/research with review | Aggregating public facts to stalk, dox, blackmail, or harass a private individual |
| Password-reuse *awareness* checks on your own accounts | Using found credentials against a real account |

**The technique is often identical. The difference is *authorization*,
*intent*, and *what you do with the result*.**

## 9.2 Laws Every OSINT Practitioner Should Know

- **India — Information Technology Act, 2000 (as amended):**
  - Section 43 / 66 — unauthorized access, data theft, introducing malware/keyloggers
  - Section 66C — identity theft
  - Section 66E — violation of privacy (capturing/publishing private images)
  - Section 354D (IPC/BNS equivalent) — cyberstalking
  - Section 507/503 — criminal intimidation via anonymous/electronic means (relevant to blackmail)
- **United States — Computer Fraud and Abuse Act (CFAA)** — criminalizes
  unauthorized access to protected computers/accounts
- **EU — GDPR** — even *aggregating* public personal data into a profile can
  trigger obligations/liability if done for non-exempt purposes
- **General** — most countries have anti-stalking, anti-harassment, and
  extortion/blackmail statutes that apply regardless of whether the
  underlying data was "public"

## 9.3 Why "It Was Public" Is Not a Legal Defense
Courts increasingly recognize the **mosaic theory of privacy**: combining many
individually-public data points into a detailed profile of a private person
can itself constitute an actionable privacy harm or enable a crime (stalking,
harassment), even though no single data point was secret. Aggregation +
targeting a real, identifiable private individual without legitimate purpose
is the risk zone.

## 9.4 What Actually Gets People Prosecuted (Illustrative, Not Instructional)
These are described at the level of *what happened and what the consequence
was* — not how to replicate them:
- Individuals who used "free WiFi tracking link" tools (disguised redirect
  links) to covertly capture a target's GPS/IP without consent have faced
  charges under unauthorized-access and stalking statutes in multiple
  jurisdictions.
- People who compiled OSINT-derived personal details (address, workplace,
  routine) about an ex-partner or public figure and published/sent them with
  intent to intimidate have been charged with cyberstalking/criminal
  intimidation, independent of whether the source data was public.
- Individuals who used breach-database credentials (found via "email OSINT")
  to actually log into someone's account have been prosecuted for
  unauthorized computer access — the *lookup* was legal; the *login* was not.

## 9.5 A Practical Decision Checklist Before Any OSINT Action
Ask yourself, in order:
1. **Do I have authorization** (written scope, consent, or clear public-interest/
   journalistic justification with editorial review)?
2. **Am I only viewing, not accessing** anything behind a login/paywall/auth
   barrier I wasn't given credentials for?
3. **Would the subject reasonably expect this level of scrutiny** given what
   they shared and where?
4. **What will I do with this information** — and would that use be legal and
   ethical even if the collection was?
5. If any answer is "no" or "I'm not sure" — **stop and don't proceed.**

## 9.6 Reporting, Not Exploiting
If your OSINT work uncovers a real vulnerability (exposed file, misconfigured
server, leaked credentials for an organization), the ethical and legal path is
**responsible disclosure** to the affected organization or a recognized bug
bounty program — not personal use of the finding.

---
**Bottom line:** the skills in Modules 01–08 are dual-use. What separates a
cybersecurity professional from a criminal is scope, consent, and intent —
every time, no exceptions.
