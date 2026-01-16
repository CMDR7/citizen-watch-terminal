

# CITIZEN — Pre-Crime Hotspot Scanner

**CITIZEN** is a single-page, client-side web application that visualizes **potential crime hotspots** using publicly available data sources and optional third-party APIs. It presents aggregated, probabilistic risk signals in a retro-CRT cyberpunk interface.

This project is a **frontend prototype** focused on transparency, ethics, and exploratory analysis—not prediction of individual behavior.

---

## What This App Does

* Accepts a city or location as input
* Geocodes the location using OpenStreetMap (Nominatim)
* Aggregates crime-related signals from:

  * Open police data (where available)
  * News and public media chatter
  * Optional third-party crime APIs
* Computes **risk scores by category** using a simple weighted model
* Displays:

  * A map with a hotspot reticule
  * Ranked crime categories
  * Confidence levels
  * Data source attribution
* Falls back to **Demo Mode** when live APIs are unavailable

All computation happens **entirely in the browser**.

---

## Architecture (Important)

* **Single file app** (`index.html`)
* No backend
* No server
* No database
* No user accounts
* No tracking
* No personal data processing

The app runs on **GitHub Pages or any static web host**.

Users may optionally supply **their own API keys**, which are stored **locally in their browser only** (`localStorage`).

---

## Supported Data Sources

### No API Key Required

* OpenStreetMap Nominatim (geocoding)
* data.police.uk (England & Wales street-level crime)

### Optional (User-Supplied API Keys)

* CrimeoMeter
* NewsAPI.org
* GNews.io

If no keys are provided or APIs fail, the app automatically switches to **Demo Mode**.

---

## Ethics & Limitations

* This tool **does not identify individuals**
* Outputs are **probabilistic**, not predictive
* Data sources may contain bias or reporting gaps
* Results should be used for **awareness and exploration only**
* Always cross-check with official local information

The UI intentionally includes a **transparent method readout** to discourage blind trust.

---

## How to Use

1. Open the app in a browser
2. Enter a city and country (e.g. `London, UK`)
3. Click **SCAN**
4. (Optional) Open ⚙ Settings and add API keys
5. Review ranked categories, confidence, and hotspots

No installation required.

---


## Disclaimer

This project is a **technical and design prototype**.

It is not:

* A law enforcement tool
* A predictive policing system
* A surveillance platform

Use responsibly.

---
## Art__

Grid’s clean. Documentation synced.

