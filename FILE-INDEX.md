# File Index – Stress Tracker Project

Complete inventory and description of all project files.

---

## 📁 Project Structure

```
/workspaces/project/
├── stress-tracker.html          [MAIN APPLICATION]
├── README.md                    [Project overview]
├── plan.md                      [Implementation roadmap & phases]
├── HARNESS.md                   [Deployment & development guide]
├── WORKLOG.md                   [Development session history]
├── CHANGELOG.md                 [Version history & changes]
├── TODO.md                      [Task tracking & remaining work]
└── FILE-INDEX.md               [This file]
```

---

## 📄 File Descriptions

### **stress-tracker.html** (Main Application)
**Type:** HTML5 + CSS3 + JavaScript  
**Size:** ~15 KB  
**Purpose:** Complete single-page stress tracking application  

**Contains:**
- Responsive HTML structure
- Embedded CSS (gradient design, mobile-first)
- Embedded JavaScript with:
  - Form validation logic
  - Stress classification engine (60+ keywords)
  - User summary generator
  - Researcher record generator
  - localStorage management
  - Entry history display

**How to Use:**
- Open directly in browser (double-click or drag to browser)
- Or use local server: `python3 -m http.server 8000`
- Visit: `http://localhost:8000/stress-tracker.html`

**Key Functions:**
- `classifyStressor(stressor)` – Categorizes stressor input
- `generateUserSummary(data, category)` – Creates personalized summary
- `generateResearcherRecord(data, category)` – Creates structured JSON
- `saveToHistory(data, category)` – Saves entry to localStorage
- `loadHistory()` – Retrieves saved entries
- `clearHistory()` – Deletes all saved entries

**Browser Support:** All modern browsers (Chrome, Firefox, Safari, Edge)

---

### **README.md** (Project Overview)
**Type:** Markdown  
**Purpose:** High-level project description and quick start guide  

**Contains:**
- Project summary
- Key features
- Quick start instructions
- Technology stack
- File structure overview

---

### **plan.md** (Implementation Roadmap)
**Type:** Markdown  
**Purpose:** Detailed implementation phases and timeline  

**Contains:**
- 7 implementation phases:
  1. Setup
  2. Form Development
  3. Core Functionality
  4. Output Display
  5. Storage (Optional)
  6. Styling & Cleanup
  7. Testing & Debugging
- Timeline estimates
- Success criteria
- Risk mitigation strategies

**Read this for:** Understanding project phases and development sequence

---

### **HARNESS.md** (Deployment & Development Guide)
**Type:** Markdown  
**Purpose:** Complete project launch, deployment, and development guide  

**Contains:**
- **Quick Start:** How to run the application
- **Implementation Status:** Completion checklist for all 7 phases
- **Feature Checklist:** All delivered features
- **Testing Scenarios:** 5 comprehensive test cases
- **Stress Categories:** Keyword reference (60+ keywords)
- **Development Guide:** How to customize and extend
- **Deployment Options:** GitHub Pages, Netlify, Vercel, traditional hosting
- **Troubleshooting:** Common issues and solutions
- **Success Criteria:** How to validate the application

**Read this for:** Running, testing, and deploying the application

---

### **WORKLOG.md** (Development Session History)
**Type:** Markdown  
**Purpose:** Track development progress and session activities  

**Contains:**
- Session dates and durations
- Tasks completed in each session
- Key decisions made
- Testing results
- Files created or modified
- Next steps and notes

**Read this for:** Understanding development history and progress

---

### **CHANGELOG.md** (Version History)
**Type:** Markdown  
**Purpose:** Document all changes, additions, and fixes by version  

**Contains:**
- **v1.0.0 (Current)**
  - All implemented features
  - Technical details
  - Testing summary
  - Deployment options
- **Known Limitations**
- **Future Enhancements**
- **Versioning Strategy** (Semantic Versioning)

**Read this for:** Understanding what changed between versions

---

### **TODO.md** (Task Tracking)
**Type:** Markdown  
**Purpose:** Organized task list for ongoing and future work  

**Contains:**
- **High Priority:** Testing scenarios and bug fixes
- **Medium Priority:** UX improvements and features
- **Low Priority:** Future enhancements (backend, analytics, mobile)
- **Completed Tasks:** ✅ Already finished
- **Notes:** Blockers, dependencies, time estimates

**Read this for:** Next tasks to complete and project roadmap

---

### **FILE-INDEX.md** (This File)
**Type:** Markdown  
**Purpose:** Complete inventory of all project files  

**Contains:**
- Project structure diagram
- File descriptions
- File purposes and contents
- How to use each file
- Cross-references

**Read this for:** Finding the right file and understanding file organization

---

## 🗂️ File Organization Strategy

### By Purpose
| Purpose | Files |
|---------|-------|
| **Application** | stress-tracker.html |
| **Documentation** | README.md, plan.md, HARNESS.md |
| **Project Management** | WORKLOG.md, CHANGELOG.md, TODO.md |
| **Reference** | FILE-INDEX.md |

### By Audience
| Audience | Core Files |
|----------|-----------|
| **End Users** | stress-tracker.html, README.md |
| **Developers** | stress-tracker.html, HARNESS.md, plan.md |
| **Project Managers** | WORKLOG.md, TODO.md, CHANGELOG.md |
| **Researchers/Analysts** | HARNESS.md (researcher output format) |

### By Update Frequency
| Frequency | Files |
|-----------|-------|
| **Static** | plan.md, README.md |
| **Regular Updates** | WORKLOG.md, TODO.md, CHANGELOG.md |
| **Rarely Changed** | FILE-INDEX.md, HARNESS.md |
| **Active Development** | stress-tracker.html |

---

## 📊 File Statistics

| File | Type | Lines | Approx. Size |
|------|------|-------|--------------|
| stress-tracker.html | HTML/CSS/JS | 350+ | 15 KB |
| HARNESS.md | Markdown | 200+ | 12 KB |
| plan.md | Markdown | 100+ | 6 KB |
| WORKLOG.md | Markdown | 60+ | 3 KB |
| CHANGELOG.md | Markdown | 120+ | 7 KB |
| TODO.md | Markdown | 150+ | 8 KB |
| FILE-INDEX.md | Markdown | 250+ | 10 KB |
| **TOTAL** | — | **1,200+** | **61 KB** |

---

## 🔄 File Dependencies

```
stress-tracker.html (MAIN)
│
├── uses logic from: (embedded JavaScript)
│   ├── Classification engine
│   ├── localStorage API
│   └── DOM manipulation
│
├── references in: HARNESS.md, plan.md
├── documented in: README.md
└── tracked in: WORKLOG.md, CHANGELOG.md, TODO.md
```

---

## 🚀 Quick File Navigation

**Want to...**
- Run the app? → Open [`stress-tracker.html`](stress-tracker.html)
- Understand phases? → Read [`plan.md`](plan.md)
- Deploy to production? → Follow [`HARNESS.md`](HARNESS.md)
- See what changed? → Check [`CHANGELOG.md`](CHANGELOG.md)
- Find next tasks? → Review [`TODO.md`](TODO.md)
- Check progress? → Read [`WORKLOG.md`](WORKLOG.md)
- Customize the app? → Edit [`stress-tracker.html`](stress-tracker.html)
- Add new features? → Update [`TODO.md`](TODO.md) + edit app + update [`CHANGELOG.md`](CHANGELOG.md)

---

## 📝 Maintenance & Conventions

### Update Guidelines
1. **stress-tracker.html:** Update after bug fixes or feature additions
2. **WORKLOG.md:** Add entry for each development session
3. **CHANGELOG.md:** Update with each version/release
4. **TODO.md:** Maintain as tasks complete or new tasks arise
5. **plan.md:** Keep as-is unless major scope changes
6. **HARNESS.md:** Update if deployment options change

### Naming Conventions
- HTML files: lowercase with hyphens (`stress-tracker.html`)
- Markdown files: UPPERCASE for docs (`README.md`, `HARNESS.md`)
- Lowercase for changelog/tracking (`plan.md`, `worklog.md`, `todo.md`)

### File Preservation
All files are tracked in Git. Before deleting or renaming:
1. Commit current state
2. Create a new branch if making major changes
3. Update references in other files
4. Update this FILE-INDEX.md

---

## 🔗 Related Resources

- [Project README](README.md)
- [Implementation Plan](plan.md)
- [Development Harness](HARNESS.md)
- [Work Log](WORKLOG.md)
- [Change Log](CHANGELOG.md)
- [Task List](TODO.md)

---

**Last Updated:** March 31, 2026  
**Maintained By:** GitHub Copilot  
**Format Version:** 1.0
