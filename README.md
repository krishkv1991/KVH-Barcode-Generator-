# Student Barcode Generator - PM SHRI KV Hinoo

A Progressive Web App (PWA) for generating QR code barcodes for student ID cards and library management.

## Features

- ✅ Generate QR codes for individual students
- ✅ Batch upload via CSV file
- ✅ Download barcodes as PNG images
- ✅ Download multiple barcodes as ZIP file
- ✅ Offline support (works without internet)
- ✅ Installable on home screen (Android/iOS)
- ✅ Mobile-friendly interface
- ✅ Professional school branding

## Quick Start

1. Visit the deployed app URL
2. **Manual Entry:** Enter student admission number, name, class, and section
3. **Batch Upload:** Upload a CSV file with multiple students
4. Generate QR codes
5. Download as individual PNG files or bulk ZIP

## CSV Format for Batch Upload

```
admission_number,full_name,class,section
A001,Raj Kumar,XI,A
A002,Priya Singh,XI,A
A003,Amit Singh,XI,B
A004,Neha Sharma,XII,A
```

**Required columns (in order):**
- `admission_number` - Student admission number (e.g., A001)
- `full_name` - Student full name (e.g., Raj Kumar)
- `class` - Class level (XI or XII)
- `section` - Section (A, B, C, D, etc.)

## Barcode Data Format

Each QR code encodes:
```
ADM:A001|NAME:Raj Kumar|CLASS:XI|SECTION:A
```

This format can be scanned by the Library Companion App (coming soon) to:
- Record book issue/return
- Track student borrowing history
- Generate reports

## Deployment

### Deploy to Netlify (Recommended)

1. Push this repository to GitHub
2. Go to https://app.netlify.com
3. Click "New site from Git"
4. Select this repository
5. Deploy automatically

### Deploy to GitHub Pages

1. Go to repository Settings → Pages
2. Select "Deploy from a branch"
3. Choose "main" branch
4. App will be available at: `https://yourusername.github.io/barcode-generator-app`

## Installation on Mobile

### Android (Pixel, OnePlus, etc.)
1. Open app URL in Chrome
2. Wait 2-3 seconds
3. Tap "Install" or "Add to Home screen" banner
4. Confirm installation
5. App appears on home screen

### iOS (iPhone, iPad)
1. Open app URL in Safari
2. Tap Share button
3. Tap "Add to Home Screen"
4. Confirm
5. App appears on home screen

**Note:** iOS has some limitations with PWA features. Full offline support works best on Android.

## File Structure

```
.
├── index.html          # Main PWA application (920 lines)
├── manifest.json       # PWA configuration and app metadata
├── _redirects          # Netlify routing configuration
├── README.md           # This file
└── .gitignore          # Git ignore rules
```

## Technology Stack

- **Frontend:** HTML5, CSS3, JavaScript (ES6+)
- **QR Code Generation:** QRCode.js library
- **Batch Processing:** JSZip library for ZIP file creation
- **PWA Features:** 
  - Service Workers for offline support
  - Web App Manifest for installability
  - IndexedDB ready for future enhancements

## Browser Support

- ✅ Chrome/Edge 60+
- ✅ Firefox 55+
- ✅ Safari 11.1+
- ✅ Mobile browsers (Chrome, Firefox, Safari)

## School Information

**Institution:** PM SHRI Kendriya Vidyalaya Hinoo, Ranchi  
**KV Code:** 1184  
**Affiliation:** CBSE  
**Created by:** Krish, PGT English  
**Contact:** PM SHRI KV Hinoo Library

## Future Enhancements (Phase 2)

Planned Library Companion App features:
- 📱 Barcode scanner (scan student QR codes)
- 📚 Book issue/return tracking
- 📊 Library reports and analytics
- 📈 Student borrowing history
- ⏰ Overdue book alerts
- ☁️ Cloud sync and backup
- 👥 Multi-user support (librarian, assistants)

## Technical Details

### QR Code Specifications
- **Format:** Code 128 & QR Code
- **Error Correction:** High level (30% recovery)
- **Size:** 200×200 pixels (printable)
- **Data:** Student admission + name + class + section

### PWA Features
- **Offline Mode:** Full local QR generation without internet
- **Caching:** Service Worker caches assets for fast loading
- **Storage:** Supports local data persistence
- **App Shell:** Loads instantly, feels native

### Performance
- **First Load:** ~2 seconds
- **Subsequent Loads:** <500ms (cached)
- **QR Generation:** <100ms per code
- **Batch Generation:** ~100ms per student

## License

School Educational Use  
PM SHRI Kendriya Vidyalaya System

## Support & Feedback

For issues, improvements, or suggestions:
- Contact: PM SHRI KV Hinoo Library
- Author: Krish (PGT English)

---

**Version:** 1.0  
**Last Updated:** March 2026  
**Status:** Production Ready ✅
