# Module 08 — Tools, Frameworks & Automation

## Curated Toolkit by Category

### Image / Metadata
- ExifTool (CLI), exif.regex.info (web)
- FotoForensics (ELA / tamper detection)
- Google Images, TinEye, Yandex (reverse search)

### Geolocation
- Google Street View / Earth, Mapillary, SunCalc, GeoGuessr (training)

### Username / Email
- Sherlock, WhatsMyName, Hunter.io, Holehe, HaveIBeenPwned, Emailrep.io

### Social Media
- Native platform search, Facebook Graph Search dorks, TweetDeck/Advanced Search

### Domain / Infrastructure
- WHOIS, crt.sh, Wayback Machine, Shodan (view-only), SecurityTrails

### All-in-One Frameworks
- **OSINT Framework** (osintframework.com) — categorized directory of tools
- **Maltego** — visual link-analysis / relationship mapping
- **theHarvester** — email/subdomain/host harvesting from public sources
- **SpiderFoot** — automated OSINT reconnaissance aggregator

## Automation & Scripting Basics
```bash
# Example: batch WHOIS lookups
for domain in $(cat domains.txt); do
  whois "$domain" >> results.txt
done
```

Learning Python + `requests`/`BeautifulSoup` lets you build custom scrapers for
**public, permitted** data sources — always check `robots.txt` and a site's
Terms of Service before automated scraping.

## Building Your Own OSINT Lab
- Use a dedicated VM (e.g., Kali Linux) so investigative browsing stays
  isolated from your personal accounts/identity
- Use a research-only browser profile with no logged-in personal accounts
- Keep a case log (source, timestamp, screenshot, hash) for every finding —
  critical for any work that may later need to hold up as evidence

## Practice Exercise
Install the OSINT Framework bookmark set and Sherlock in a lab VM. Run a full
recon pass on a **test account you create yourself**, end to end.
