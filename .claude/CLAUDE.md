# eBay Auto-Listing Tool

## What This Is
A PWA for generating eBay listings from photos using Google Gemini AI. Single HTML file, no build step, deployed on GitHub Pages.

## Architecture
- **Single file**: `index.html` contains all HTML, CSS, and JS
- **AI**: Google Gemini 1.5 Flash via browser SDK (free tier)
- **Storage**: localStorage for drafts and settings
- **Offline**: Service worker caches app shell; drafts work offline, AI requires connection
- **Deploy**: GitHub Pages from main branch

## Key Patterns
- API key stored in localStorage (same as Field Buddy's Sheets URL pattern)
- Dark theme (#1a1a2e background)
- Mobile-first, optimized for iPhone one-handed use
- Bottom tab navigation: New Listing | Drafts | Settings

## Item Types
Appliance parts, audio cables, bulk cable, small tools, electronics

## Files
- `index.html` — The entire app
- `manifest.json` — PWA manifest
- `sw.js` — Service worker for offline support
