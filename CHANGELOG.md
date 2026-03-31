# Changelog – Stress Tracker

All notable changes to this project are documented here.

## [1.0.0] – 2026-03-31 – Initial Release

### Added
- **Core Application**
  - Single-page web application (stress-tracker.html)
  - Responsive design for desktop, tablet, mobile
  - Gradient UI with modern styling

- **Form Features**
  - Text input for name/ID
  - Text input for stressor description
  - Radio buttons for severity (1–5 scale)
  - Textarea for coping strategies
  - Textarea for emotional description
  - Form validation (required fields)
  - Reset button

- **Classification Engine**
  - Keyword-based stressor classification
  - 4 primary categories:
    - Academic (exams, deadlines, grades, studying, etc.)
    - Social (family, friends, relationships, conflicts, etc.)
    - Financial (money, bills, debt, savings, etc.)
    - Health (doctor, wellness, weight, sleep, anxiety, etc.)
  - Fallback to "Other" for unclassified stressors
  - 60+ predefined keywords

- **User Output**
  - Personalized summary with user's name
  - Category badge with emoji
  - Severity level display
  - Supportive feedback message
  - Practical suggestions for the specific category
  - Immediate display after submission

- **Researcher Output**
  - Structured JSON record
  - Fields: timestamp, name, stressor, category, severity, coping strategies, emotions
  - Pretty-printed for readability
  - Copy-friendly format

- **Data Persistence**
  - localStorage integration
  - Automatic entry saving
  - Entry history list (most recent first)
  - Timestamp for each entry
  - "Clear History" button with confirmation

- **Documentation**
  - HARNESS.md – deployment & development guide
  - plan.md – implementation roadmap
  - WORKLOG.md – development session log
  - CHANGELOG.md – version history
  - FILE-INDEX.md – project structure

### Technical Details
- **Framework:** Vanilla JavaScript, HTML5, CSS3
- **Database:** Browser localStorage
- **Backend:** None (fully client-side)
- **Dependencies:** None
- **Browser Support:** All modern browsers (Chrome, Firefox, Safari, Edge)
- **Accessibility:** Semantic HTML, clear labels, keyboard navigable

### Testing
- Form validation tested
- Classification accuracy verified (15+ test cases)
- localStorage persistence confirmed
- Responsive design validated
- No console errors

### Deployment Options
- Direct file open (drag & drop to browser)
- Local server (Python, Node.js, etc.)
- GitHub Pages
- Netlify
- Vercel
- Traditional web hosting

---

## [Unreleased] – Future Enhancements

### Planned Features
- [ ] CSV export functionality
- [ ] Dark mode toggle
- [ ] Advanced analytics dashboard
- [ ] Multiple language support
- [ ] Email summary delivery
- [ ] Integration with calendar apps
- [ ] Trend visualization (charts/graphs)
- [ ] Custom category creation
- [ ] API endpoint for data sharing
- [ ] Progressive Web App (PWA) capabilities

### Known Limitations
- Single user per browser (localStorage is per-device)
- No automatic backups (manual export recommended)
- Case-sensitive keyword matching
- No multi-language support yet

---

## Versioning
This project uses [Semantic Versioning](https://semver.org/):
- **MAJOR** version for incompatible API changes
- **MINOR** version for new functionality (backward compatible)
- **PATCH** version for bug fixes

---

## Contributors
- Project Lead & Developer: GitHub Copilot
- Requirements: Based on user specifications
