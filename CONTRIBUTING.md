# Contributing to PDF Toolkit Pro

Thanks for considering contributing! This project was built out of frustration with existing PDF tools, and I'd love to make it better with your help.

## 🤔 Before You Start

This project has one core principle: **Offline-first, privacy-focused**

Before adding any feature, ask yourself:
- Does this require a server? (If yes, it doesn't belong here)
- Does this add tracking/analytics? (Hard no)
- Does this upload files anywhere? (Absolutely not)

If you answered yes to any of these, it won't be merged. Everything must run client-side.

## 🐛 Found a Bug?

Open an issue with:
- What you were trying to do
- What happened instead
- Browser/OS you're using
- Any console errors (F12 → Console tab)

Screenshots help a lot!

## 💡 Have a Feature Idea?

Cool! Open an issue first before writing code. Let's discuss if it fits the project's philosophy.

**Good feature ideas:**
- New PDF tool (e.g., "Add Page Borders")
- Better mobile UX
- Performance improvements
- Accessibility enhancements
- Better error messages

**Feature ideas that won't work:**
- Server-side processing
- User accounts/login
- Cloud storage integration
- Paid features
- Tracking/analytics

## 🔧 Want to Contribute Code?

### The Setup (It's ridiculously simple)

1. Fork the repo
2. Download `main.html`
3. Open it in your browser
4. Edit the file
5. Refresh browser to see changes

That's it. No npm install, no build process, no webpack config. Just HTML, CSS, and JavaScript.

### Code Style

Keep it readable:
- Use meaningful variable names (not `x`, `y`, `data1`)
- Add comments for complex logic
- Keep functions focused (do one thing well)
- Don't over-engineer (vanilla JS is fine!)

### Testing Your Changes

Before submitting:
1. Test on mobile (Chrome DevTools → Mobile view)
2. Test on desktop
3. Try dark mode
4. Test with large files (catch memory issues early)
5. Check browser console for errors

### The PR Process

1. Make your changes in a fork
2. Test thoroughly
3. Open a PR with a clear description:
   - What does this fix/add?
   - How did you test it?
   - Any breaking changes?

I'll review it, probably ask questions, maybe suggest changes. Don't take it personally - I'm just trying to keep the code quality high.

## 🎨 Design Guidelines

Keep the UI:
- Clean and modern (not cluttered)
- Accessible (keyboard navigation, screen readers)
- Mobile-friendly (touch targets ≥ 44px)
- Consistent with existing style

## 🚫 What We Don't Accept

- Code with external dependencies beyond the existing CDN libraries
- Tracking/analytics code
- Server-side functionality
- Obfuscated code
- Features that only work in one browser (unless gracefully degraded)

## 📝 Documentation

If you add a feature, update the README. Keep it in the same friendly, honest tone.

## 🏆 Recognition

Contributors get added to the README's credits section. Because credit where credit's due.

## ❓ Questions?

Not sure about something? Open an issue and ask. I'd rather answer questions than review problematic PRs.

## 🙏 Thank You

Seriously, thanks for wanting to make this better. Whether you're fixing a typo in the README or adding a whole new tool, it's appreciated.

Just remember: **Offline-first. Privacy-focused. Keep it simple.**

---

**Not a coder?** You can still help by:
- Testing and reporting bugs
- Improving documentation
- Suggesting features
- Sharing the project with others who value privacy
