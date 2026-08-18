# Module 06 — Domain & Website OSINT

## Concept
Websites and domains leak organizational and personal data through
registration records, subdomains, and exposed files.

## Core Techniques
| Technique | Tool | Reveals |
|---|---|---|
| WHOIS Lookup | whois.domaintools.com, `whois` CLI | Registrant info (if not privacy-protected), registrar, dates |
| DNS Recon | dig, nslookup, SecurityTrails | Subdomains, mail servers, hosting provider |
| Wayback Machine | web.archive.org | Historical versions of a site (before edits/takedowns) |
| Certificate Transparency | crt.sh | Subdomains via SSL cert logs |
| File Discovery | Google dorking | Exposed PDFs, docs, spreadsheets |

## Google Dorking for Public Documents
```
site:gov.in filetype:pdf confidential
site:nic.in filetype:xlsx
intitle:"index of" "backup"
```

> ⚠️ Finding a publicly indexed file is legal OSINT. **Attempting to access
> anything behind a login, guessing directory paths to bypass access controls,
> or exploiting a misconfiguration to extract non-indexed data crosses into
> unauthorized access — illegal under most computer-crime laws.**

## IP & Infrastructure Intelligence
- Shodan.io — internet-connected device/service discovery (legal to *view*
  public banners; illegal to exploit or access anything requiring auth)
- BuiltWith / Wappalyzer — tech stack fingerprinting

## Practice Exercise
Run a WHOIS + Wayback Machine check on a domain you own or a well-known public
company's main site. Document what's publicly disclosed vs. privacy-protected.
