# Module 04 — Username & Email OSINT

## Concept
Most people reuse usernames and emails across platforms. A username is a
**digital fingerprint**; an email is a key that can unlock associated accounts,
breach history, and professional footprints.

## Username Search Tools
| Tool | Purpose |
|---|---|
| Sherlock | Checks a username across 300+ sites, returns live profile links |
| WhatsMyName | Similar cross-platform username search |
| NameCheckup / Namechk | Availability + presence checking |

```bash
python3 sherlock.py target_username
```

## Email Search & Breach Tools
| Tool | Purpose |
|---|---|
| Hunter.io | Finds where an email is used professionally / domain email patterns |
| Emailrep.io | Reputation checker (spam score, breach flags, trust score) |
| HaveIBeenPwned.com | **The** authoritative breach-check database |
| Holehe | Checks which of 100+ websites an email is registered on |
| h8mail | OSINT email breach hunting (aggregates multiple breach sources) |
| Socialscan | Checks email/username availability across platforms |

## Google Dorking for Username/Email Correlation
```
intext:"username123" site:github.com
"user@gmail.com" site:linkedin.com
filetype:pdf "username123"
```

## From One Username to a Fuller (Public) Picture
1. Run Sherlock → gather linked social profiles
2. Pull public profile photos → reverse image search
3. Cross-reference bio info, pinned posts, follower patterns
4. Note any **publicly stated** location/employer/hobbies
5. Cross-check email against HaveIBeenPwned for breach exposure awareness

> This entire workflow only touches **public** profile data. Never attempt to
> "recover" or reset accounts, guess security answers, or use breach data to log
> into anything — that immediately becomes unauthorized access (a crime).

## Practice Exercise
Run Sherlock and HaveIBeenPwned on your **own** username/email. Most students
are surprised how much is public — that's the point of this module: awareness.
