# Module 02 — Image OSINT: Secrets Hidden in Photos

## Concept
Every image carries potential metadata and visual clues: camera model, GPS
coordinates, timestamps, reflections, backgrounds, shadows.

## 2.1 EXIF Metadata Extraction
**Tools:** `exiftool` (CLI), exif.regex.info (web), Jeffrey's Exif Viewer

```bash
exiftool photo.jpg
```

Look for:
- 📍 GPS Latitude/Longitude
- 📷 Camera Make & Model
- 🕐 Date/Time Original
- 👤 Software / Owner metadata (sometimes)

> ⚠️ Note: Most social platforms (Instagram, WhatsApp, Facebook) **strip EXIF data**
> on upload. Raw/shared files (email attachments, unedited downloads) are more likely
> to retain it.

## 2.2 Reverse Image Search
**Tools:** Google Images, TinEye (image history/tracking), Yandex (best for faces)

**Workflow:**
1. Upload or paste image URL
2. Review indexed matches across the web
3. Identify: source platform, other appearances, associated names

## 2.3 Error Level Analysis (Detecting Fakes)
**Tool:** FotoForensics.com — detects edited/tampered regions via ELA
(compression artifact analysis).

## 2.4 Visual Forensics Checklist
- Background signage/language → narrows country/city
- Reflections in sunglasses, windows, mirrors
- Shadow direction/length → rough time of day
- Clothing style + weather visible → season/hemisphere
- Screenshots of maps → can be re-identified via reverse search of the map tile itself

## 2.5 Facial Recognition Search
Tools like FaceCheck.ID index public faces across social media, news, mugshots.

> ⚠️ **Ethics flag:** Facial recognition search on a real person without their
> knowledge is a significant privacy intrusion even when "legal" in your
> jurisdiction. Use only with consent, on public figures for journalism with
> editorial justification, or in authorized investigations.

## Practice Exercise
Take a photo you personally shot (unedited, straight off your phone/camera) and
run `exiftool` on it. Compare the GPS data to your actual location.
