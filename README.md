# 📄 PDF Toolkit Pro - Complete Offline PDF & Image Suite

A fully offline, privacy-focused web application that handles all your PDF and image processing needs right in your browser. No uploads, no servers, no tracking - just pure client-side magic.

## 🎯 Why I Built This

I got tired of sketchy online PDF tools that either:
- Upload your files to unknown servers (goodbye privacy!)
- Require subscriptions for basic features
- Work terribly on mobile
- Have annoying file size limits

So I built this - everything runs locally in your browser. Your files never leave your device. Period.

## ✨ What It Does

### PDF Tools (15 in total)
- **✍️ Sign PDF** - Draw or type your signature, drag & drop it anywhere
- **📝 Extract Text** - Copy text from PDFs with full formatting
- **💧 Watermark** - Add custom text overlays
- **🔄 Image & PDF Converter** - Convert between JPG, PNG, WebP, and PDF (handles up to 10 files)
- **✨ Image Optimizer** - Smart compression with presets (Document, Photo, Web)
- **🔢 Page Numbers** - Auto-number your pages
- **✂️ Split PDF** - Extract specific pages (visual selection or range input)
- **📑 Merge PDFs** - Drag to reorder, then combine
- **🔄 Rotate PDF** - Fix orientation page-by-page or all at once
- **🗑️ Delete Pages** - Click to remove unwanted pages
- **👁️ OCR** - Extract text from images (uses Tesseract.js)
- **🏷️ Metadata** - Edit PDF title, author, etc.
- **📄 Text to PDF** - Convert notes to documents
- **📦 Compress PDF** - Two modes: Structure optimization or aggressive image compression with color controls (Color/Grayscale/B&W)

### Smart Features
- **Dark Mode** - Easy on the eyes
- **Mobile-Friendly** - Touch-optimized interface with larger buttons
- **Processing Locks** - Prevents you from breaking things by clicking twice
- **Smart Download System** - Desktop users get a choice (ZIP or individual files), mobile gets optimized downloads
- **Safety Limits** - Won't let you process 500-page PDFs and crash your browser
- **Helpful Guidance** - Modals that actually help instead of confuse

## 🚀 How to Use

### Option 1: Download and Use Locally
1. Download `main.html`
2. Open it in your browser
3. That's it. Seriously.

No server needed, no installation, no npm packages. Just open the file and you're ready to go.

### Option 2: Host It Yourself
Upload to any static hosting (GitHub Pages, Netlify, Vercel, or even a USB drive):
```bash
# Just upload the HTML file - that's all you need
```

## 🛠️ Technical Stuff (For Fellow Devs)

### Built With
- Pure vanilla JavaScript (no frameworks - keeping it simple)
- [pdf-lib](https://pdf-lib.js.org/) - PDF manipulation
- [PDF.js](https://mozilla.github.io/pdf.js/) - PDF rendering
- [JSZip](https://stukjs.github.io/jszip/) - ZIP file creation
- [Tesseract.js](https://tesseract.projectnaptha.com/) - OCR

### Architecture Highlights
- **6,630 lines** of carefully crafted code
- **Offline-first** - Zero server dependencies
- **Processing locks** - Prevents race conditions and double-clicks
- **Memory management** - Proper cleanup with URL.revokeObjectURL
- **Error handling** - Comprehensive try-catch with user-friendly messages
- **Progressive enhancement** - Works on mobile, better on desktop

### Smart Design Decisions
1. **Image Converter** merges image-to-image AND PDF-to-image conversion
2. **Compression has two modes** - lossless structure optimization OR aggressive image compression
3. **Safe limits** - 10-image limit for converters, 300-page block for PDFs
4. **Aurora gradient background** - Only on desktop (mobile gets clean UI)
5. **Processing state management** - Locks UI during operations to prevent chaos

## 🎨 Design Philosophy

**Simple but not simplistic.** 

I wanted professional-grade tools that don't overwhelm casual users. So:
- Clean, modern UI that doesn't look like it's from 2005
- Helpful tooltips and warnings (not annoying ones)
- Smart defaults (you can convert images without touching any settings)
- Advanced options when you need them (color modes, quality presets, page ranges)

## 🔒 Privacy

Your files stay on your device. No tracking, no analytics, no servers. 

Want proof? Open DevTools → Network tab. You'll see the libraries load from CDNs, then nothing. Because there's nothing to send.

## 📱 Mobile Experience

This isn't just "mobile responsive" - it's actually redesigned for mobile:
- Larger touch targets (44px minimum)
- Collapsible sections to reduce scrolling
- Optimized layouts (no horizontal scrolling)
- Smart defaults for mobile users (auto-ZIP on desktop, individual downloads on mobile)

## 🐛 Known Limitations

Let's be honest about what this can't do:

1. **HEIC files** - Browsers don't support them natively (convert to JPG first)
2. **Huge PDFs** - Blocked at 300 pages to prevent browser crashes
3. **Very large images** - 16MP safety limit to avoid memory issues
4. **Batch processing 100+ files** - You'll get a warning (browser limitations)

These aren't bugs - they're safety guardrails.

## 🤝 Contributing

Found a bug? Have an idea? Want to add a feature?

Feel free to:
- Open an issue
- Submit a PR
- Fork it and make it your own

Just keep the offline-first philosophy. No tracking, no servers.

## 📜 License

MIT - Do whatever you want with it. Just don't blame me if something breaks.

## 💭 Final Thoughts

I built this for myself and figured others might find it useful. It's not perfect, but it works well and respects your privacy.

If you use it and find it helpful, star the repo. If you find bugs, let me know. If you want to improve it, go ahead.

---

**Made with ☕ and frustration with existing PDF tools**

No frameworks were harmed in the making of this project.
