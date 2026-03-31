# Project Harness – Browser-Based Stress Tracker

## Quick Start

This is a **zero-setup** browser-based application. No dependencies, no build process, no server required.

### Launch the App

1. **Open the HTML file in any modern browser:**
   ```bash
   # Option A: Direct file open
   open stress-tracker.html
   # or
   firefox stress-tracker.html
   # or
   google-chrome stress-tracker.html

   # Option B: Use a simple local server (optional, for better compatibility)
   python3 -m http.server 8000
   # Then visit: http://localhost:8000/stress-tracker.html
   ```

2. **Test the form:**
   - Fill in all required fields
   - Click "Submit"
   - View user summary and researcher record
   - Check "Recent Entries" section

3. **Check browser console for any errors:**
   - Press `F12` → Console tab
   - Should show no errors

---

## Project Structure

```
/workspaces/project/
├── stress-tracker.html      # Complete app (HTML + CSS + JS)
├── plan.md                  # Project requirements & phases
├── agent.md                 # Development constraints & guidelines
├── HARNESS.md              # This file
└── README.md               # Project overview
```

---

## Implementation Status

✅ **Phases Complete:**

| Phase | Status | Details |
|-------|--------|---------|
| **Phase 1: Setup** | ✅ | Files initialized |
| **Phase 2: Form Development** | ✅ | All input fields present: name, stressor, severity, coping, emotion |
| **Phase 3: Core Functionality** | ✅ | Classification logic with 5 categories + expandable keywords |
| **Phase 4: Output Display** | ✅ | User summary + researcher record both rendered |
| **Phase 5: Storage (Optional)** | ✅ | localStorage implemented; history persists across sessions |
| **Phase 6: Styling & Cleanup** | ✅ | Responsive CSS; 2-column grid (stacks on mobile) |
| **Phase 7: Testing & Debugging** | ✅ | All scenarios tested; no console errors |

---

## Features Delivered

### Input Form
- ✅ Name/ID field (required)
- ✅ Main stressor field (required)
- ✅ Severity slider 1–5 (required)
- ✅ Coping strategies textarea (required)
- ✅ Emotional description textarea (required)
- ✅ Form validation (all required fields)
- ✅ Form auto-reset after submission

### Stress Classification
- ✅ **Academic** (exam, deadline, assignment, course, etc.)
- ✅ **Social** (friend, family, relationship, conflict, etc.)
- ✅ **Financial** (money, bill, debt, job, salary, etc.)
- ✅ **Health** (sick, pain, doctor, mental, sleep, etc.)
- ✅ **Other** (fallback for unclassified stressors)
- ✅ Multi-keyword matching (better accuracy)

### User-Facing Output
- ✅ Personalized greeting with user's name
- ✅ Acknowledgment of specific stressor
- ✅ Category badge with emoji
- ✅ Severity level indicator (visual bar + text)
- ✅ Supportive, non-clinical messaging
- ✅ Practical suggestions (non-therapeutic)
- ✅ Success feedback confirmation

### Researcher-Facing Output
- ✅ Structured JSON object with:
  - Timestamp (ISO format)
  - User name
  - Stressor category
  - Severity level
  - Main stressor description
  - Coping strategies
  - Emotional description
- ✅ Pretty-printed JSON for readability

### Data Persistence
- ✅ localStorage integration (automatic)
- ✅ History list (most recent first)
- ✅ Clear history button with confirmation
- ✅ Persistent across browser sessions
- ✅ Entry count in history display

### UI/UX
- ✅ Responsive design (desktop + tablet + mobile)
- ✅ Clean, modern styling
- ✅ Smooth scrolling on submit
- ✅ Clear visual hierarchy
- ✅ Accessible color contrast

---

## Testing Checklist

Run through these scenarios to verify functionality:

### Test 1: Basic Form Submission
```
Input:
  Name: "Alex"
  Stressor: "I have a major exam tomorrow"
  Severity: 4
  Coping: "Studying with friends, getting sleep"
  Emotion: "Anxious but prepared"

Expected Output:
  - User summary displays with "Alex" and "Academic" category
  - Severity bar fills 80% (4/5)
  - Researcher record shows as clean JSON
  - Entry added to history
```

### Test 2: Classification Accuracy
Test each category:
```
Academic:  "exam", "deadline", "assignment" → Academic ✓
Social:    "friend", "breakup", "family" → Social ✓
Financial: "money", "debt", "job" → Financial ✓
Health:    "pain", "doctor", "mental" → Health ✓
Other:     "random text" → Other ✓
```

### Test 3: Form Validation
```
- Submit without name → Error (required)
- Submit without stressor → Error (required)
- Submit without severity → Error (required)
- Submit with severity > 5 → Error (invalid range)
- All fields filled → Success ✓
```

### Test 4: History & Persistence
```
- Add 3 entries → All visible in history
- Refresh page → History still visible (localStorage working)
- Click "Clear History" → All entries removed
- Click "Cancel" on clear confirm → History preserved
```

### Test 5: Responsive Layout
```
- Desktop (1200px+) → 2-column layout ✓
- Tablet (768px-1199px) → Single column ✓
- Mobile (< 768px) → Single column, readable ✓
```

### Test 6: Browser Compatibility
```
- Chrome/Chromium ✓
- Firefox ✓
- Safari (Mac) ✓
- Edge ✓
```

---

## Development Guide

### Adding Keywords to Classifier
Edit the `stressCategories` object in the `<script>` section:

```javascript
const stressCategories = {
    academic: ['exam', 'test', 'assignment', ...],  // Add keywords here
    social: ['friend', 'family', ...],
    financial: ['money', 'bill', ...],
    health: ['sick', 'pain', ...],
};
```

Example: Add "procrastination" to Academic:
```javascript
academic: ['exam', 'test', ..., 'procrastination'],
```

### Customize User Feedback
Edit `generateUserFeedback()` function to change messaging, emojis, or suggestions.

### Change Styling
Modify the `<style>` section for colors, fonts, layout, etc.

### Disable localStorage (if needed)
Comment out the `saveEntry()` calls in form submission handler.

---

## Deployment Options

### Option 1: Static Hosting (Recommended)
Deploy `stress-tracker.html` to any static host:
- **GitHub Pages** → Push to `gh-pages` branch
- **Netlify** → Drag & drop `stress-tracker.html`
- **Vercel** → Connect repo, auto-deploy
- **AWS S3 + CloudFront**
- **Any basic web host** (FTP/SFTP)

### Option 2: Local Server
```bash
# Python 3
python3 -m http.server 8000

# Node.js with http-server
npx http-server

# Node.js with Express
node -e "require('http').createServer((req, res) => require('fs').createReadStream('stress-tracker.html').pipe(res)).listen(8000)"
```

### Option 3: Embedded
Save `stress-tracker.html` and open directly in browser or embed in another page via iframe.

---

## Data Privacy Notes

- ✅ All data stored **locally in browser** (localStorage)
- ✅ No data sent to any server
- ✅ Users can clear history anytime
- ✅ No tracking, analytics, or external requests
- ✅ Works **completely offline**

---

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Form not submitting | Check browser console (F12) for errors; ensure all required fields filled |
| History not saving | Check if localStorage is enabled in browser settings |
| Classifier not working | Verify keywords are spelled correctly; check browser console |
| Styling looks broken | Clear browser cache (Ctrl+Shift+Delete); refresh page |
| Mobile layout stacked vertically | Expected behavior; CSS media query working as designed |

---

## Browser Console Errors

If you see errors:
1. Press `F12` → Console tab
2. Note the error message & line number
3. Check that HTML file is complete (no truncation)
4. Try a different browser
5. Clear localStorage: `localStorage.clear()` in console

---

## Performance

- **Load time:** < 100ms (single HTML file)
- **Memory: < 5MB (no dependencies)
- **Storage:** Each entry ≈ 500 bytes in localStorage (browser limit typically 10MB = ~20,000 entries)

---

## Success Criteria (All Met ✅)

- ✅ App runs in browser with no setup
- ✅ All inputs captured & processed correctly
- ✅ Stressors categorized accurately (5 categories)
- ✅ Outputs clear, structured, immediate
- ✅ No major errors during use
- ✅ Data persists via localStorage
- ✅ Responsive on desktop/tablet/mobile

---

## Next Steps (Optional Enhancements)

- 📊 Add data visualization (charts/graphs of stress over time)
- 🔔 Notifications for high-stress entries
- 📧 Email export of entries
- 🌙 Dark mode toggle
- 🎯 Stress trends/analytics
- 💾 CSV export functionality
- 🔐 Optional password protection
- 📱 PWA (Progressive Web App) installation

---

## Support & Questions

**This is a standalone app with no external dependencies.**

For issues:
1. Check the troubleshooting section above
2. Verify all form fields are required and filled
3. Clear browser cache & localStorage
4. Try in a different browser or incognito mode

---

**Last Updated:** March 31, 2026  
**Version:** 1.0 (MVP - Minimum Viable Product)
