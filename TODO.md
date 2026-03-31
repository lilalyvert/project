# TODO List – Stress Tracker

## Current Phase: Quality Assurance & Feedback

### High Priority (Phase 8 – Testing & Debugging)
- [ ] **Manual Testing – All Input Scenarios**
  - [ ] Test with valid inputs across all categories
  - [ ] Test with missing required fields (should show error)
  - [ ] Test with edge cases (very long text, special characters)
  - [ ] Test severity selection (all 5 options)
  - [ ] Test form reset functionality
  
- [ ] **Classification Accuracy**
  - [ ] Verify "exam" classified as Academic
  - [ ] Verify "friend conflict" classified as Social
  - [ ] Verify "rent due" classified as Financial
  - [ ] Verify "doctor appointment" classified as Health
  - [ ] Test keyword combinations for better categorization

- [ ] **Browser Compatibility**
  - [ ] Test on Chrome (latest)
  - [ ] Test on Firefox (latest)
  - [ ] Test on Safari (latest)
  - [ ] Test on Edge (latest)
  - [ ] Test on mobile browsers

- [ ] **Responsive Design**
  - [ ] Verify mobile layout (320px–480px)
  - [ ] Verify tablet layout (768px–1024px)
  - [ ] Verify desktop layout (1200px+)
  - [ ] Test touch interactions on mobile

- [ ] **Console & Errors**
  - [ ] Verify no JavaScript errors in console
  - [ ] Verify no warnings in console
  - [ ] Test localStorage quota (exceeded storage scenario)

- [ ] **Data Persistence**
  - [ ] Submit multiple entries and verify all save
  - [ ] Verify history displays in reverse chronological order
  - [ ] Test "Clear History" button
  - [ ] Test page reload (history should persist)
  - [ ] Test across multiple browser sessions

### Medium Priority (Phase 7 – Optional Enhancements)

- [ ] **User Experience Improvements**
  - [ ] Add loading indicator for form submission
  - [ ] Add success toast/notification after submission
  - [ ] Improve error message clarity
  - [ ] Add keyboard shortcuts (Enter to submit, Esc to reset)

- [ ] **Advanced Features**
  - [ ] CSV export of entries
  - [ ] JSON export for analysis
  - [ ] Date range filtering for history
  - [ ] Search history by keyword
  - [ ] Edit/delete individual entries

- [ ] **Styling Enhancements**
  - [ ] Add animations for output appearance
  - [ ] Implement dark mode toggle
  - [ ] Improve print styling
  - [ ] Add accessibility improvements (WCAG AA compliance)

### Low Priority (Future Releases)

- [ ] **Backend Integration** (if required)
  - [ ] Design API endpoints
  - [ ] Implement user authentication
  - [ ] Create database schema
  - [ ] Add server-side validation

- [ ] **Analytics & Reporting**
  - [ ] Dashboard with stress trends
  - [ ] Category distribution charts
  - [ ] Severity trends over time
  - [ ] Coping strategy effectiveness tracking

- [ ] **Collaboration Features**
  - [ ] Share entries with therapist/coach
  - [ ] Multi-user support (with login)
  - [ ] Team stress tracking
  - [ ] Comments & feedback system

- [ ] **Mobile App**
  - [ ] React Native or Flutter implementation
  - [ ] Push notifications
  - [ ] Offline functionality
  - [ ] Native mobile UI

### Completed Tasks ✅
- [x] Phase 1: Setup and HTML structure
- [x] Phase 2: Form development with validation
- [x] Phase 3: Core JavaScript functionality
- [x] Phase 4: Output display (user summary & researcher record)
- [x] Phase 5: Storage implementation (localStorage)
- [x] Phase 6: Styling and responsiveness
- [x] Create project documentation (plan, harness, worklog, changelog)

---

## Notes
- **Blockers:** None currently
- **Dependencies:** None (fully client-side)
- **Estimated Time to Phase 8 Complete:** 2–4 hours additional testing
- **Success Criteria:** All high-priority items completed + zero console errors
