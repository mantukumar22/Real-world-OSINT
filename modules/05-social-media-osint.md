# Module 05 — Social Media OSINT (Ethically)

## Concept
Social platforms are the largest voluntary self-disclosure databases in human
history. The skill is reading what's already shared, not breaking in.

## Facebook OSINT Checklist
- Full name + username + profile URL
- Education, workplace, hometown, current city (if public)
- DP/cover photo → reverse image search for reuse elsewhere
- Mutual friends → relationship mapping
- Public posts → opinions, tagged photos, check-ins

## Facebook Dorking Examples
```
site:facebook.com "lives in Mumbai" "works at TCS"
site:facebook.com "username.here" "likes" "Bangalore"
site:facebook.com "joined in 2020" "studied at Delhi University"
```

## Instagram / LinkedIn Considerations
- Instagram: story highlights, tagged location, geotags in captions
- LinkedIn: employment history, connections graph, endorsements/skills

## Case Study — How Small Clues Compound
A person posts a pet photo → background reveals a society/apartment complex
name → a second post is geotagged by a friend → comments reveal the building
name → combined, four public posts triangulate a home address.

**This is presented as a cautionary example, not a target list.** The lesson:
*your own* scattered "harmless" posts can be aggregated the same way. That's
why OPSEC (Module 10) matters as much as offensive technique.

## Ethical Line
| OK | Not OK |
|---|---|
| Reading a public post | Requesting to "friend" solely to access private data |
| Noting publicly listed employer | Using found info to contact/harass someone |
| Journalistic verification of a public figure's claim | Building a dossier on a private individual "for fun" |
| Reporting a fake/scam account to the platform | Impersonating someone to social-engineer their contacts |

## Practice Exercise
Audit your **own** Facebook/Instagram profile as if you were a stranger doing
recon on you. Screenshot everything a stranger could learn in 5 minutes. Then
go lock it down (see Module 10).
