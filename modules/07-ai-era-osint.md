# Module 07 — OSINT in the AI Era

## Why This Module Exists
AI has changed both **how OSINT is performed** and **how hard it is to trust
what you find**. A modern OSINT practitioner must understand both sides.

## 7.1 AI as an OSINT Force Multiplier
| AI Capability | OSINT Application |
|---|---|
| LLM-assisted query generation | Faster Google dork construction, cross-language search terms |
| AI reverse-image / facial clustering | Faster face-matching across large datasets (raises major privacy concerns) |
| Satellite image analysis (ML) | Automated change-detection (used by Bellingcat, Planet Labs analysts) |
| Speech-to-text + translation | Rapid processing of foreign-language video/audio evidence |
| Sentiment/network analysis | Mapping disinformation spread across social platforms |
| AI geolocation assistants (e.g., GeoSpy-style tools) | Suggests likely locations from visual cues — **must be human-verified**, not trusted blindly |

## 7.2 The New Risks: AI Makes Deception Cheaper
- **Deepfakes** — fabricated video/audio of real people. OSINT verification now
  requires deepfake-detection literacy (frame artifacts, blink patterns,
  audio-lip sync mismatches, provenance metadata like C2PA).
- **AI-generated fake profiles** — entire synthetic personas with AI-generated
  face photos (spot via GAN-artifact detectors, reverse image search often
  returns *no* prior matches for synthetic faces — itself a signal).
- **AI voice cloning** — used in scams/vishing; OSINT analysts must verify
  audio provenance before treating it as evidence.
- **Data poisoning of AI search summaries** — AI-generated search overviews can
  hallucinate facts; always verify against a primary source.

## 7.3 Practical AI-Era OSINT Verification Checklist
1. Never trust a single AI-generated summary as a source — trace back to origin
2. Reverse image search AI-suspected content on multiple engines (Google,
   Yandex, TinEye)
3. Check for metadata/provenance signals (C2PA content credentials where present)
4. Cross-verify claims across at least two independent sources
5. Be skeptical of "too clean" or context-free viral content

## 7.4 Using AI Assistants Responsibly in OSINT Work
- Good use: summarizing large sets of *already-collected* public data, drafting
  dork queries, translating foreign-language sources, organizing timelines
- Bad use: asking an AI to generate personal profiles of real private
  individuals, to "guess" private information, or to help access non-public
  data — legitimate AI tools (including this one) will and should refuse this

## Practice Exercise
Find a viral image/video online and run it through a full AI-era verification
pass (reverse image search + metadata check + cross-source check). Document
whether it holds up.
